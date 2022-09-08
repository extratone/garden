---
{"dg-publish":true,"permalink":"/snippets/save-drafts-from-date/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# Save Drafts from Date 
Updated `08202022-153019`

[Drafts Directory: save drafts from date - text dates](https://actions.getdrafts.com/a/2CF)

- [Drafts](drafts://open?uuid=CAABBB06-186C-437D-BC30-65844BDBEC2B)
- [WTF](https://davidblue.wtf/drafts/CAABBB06-186C-437D-BC30-65844BDBEC2B.html)
- Simplenote Local
- Simplenote Publish
- Things

---

```js
// today_to_file.js
var datename='',drArr=[],t='';
var day = new Date(),tnote='',fm='';
var divider = "\n<><><><><><><><>\n" // will be placed between drafts when consolidated inot one file

var p = Prompt.create();
p.title = "Consolidate day(s) drafts";
p.message = "(defaults to today)";
//
//set choices in picker
p.addTextField("strtDate", "Start date (yyyy-mm-dd)", strftime(day,"%Y-%m-%d") );
p.addTextField("endDate","End date (yyyy-mm-dd)",strftime(day,"%Y-%m-%d"));
p.addSwitch("sw2","modifiedAt  <-  vs.  ->  createdAt",false)
p.addSwitch("sw1","early_1st  <-  vs.  ->  later_1st",false)
p.addSelect("loc","location:",["all","inbox","archive","trash"],["inbox"], false)
p.addTextField("tgs", "if desired, by Tags (ALL REQD):", "");
p.addTextField("ogs", "if desired, OMIT these Tags:", "");
// a final "go" button
p.addButton("Consolidate drafts");
// now show and choose
var didSelect = p.show();
//
//collect the values from the prompt:
var locat = p.fieldValues["loc"];
var qTags = p.fieldValues["tgs"];
var oTags = p.fieldValues["ogs"];
var sortBy = p.fieldValues["sw2"];
var sortTime = p.fieldValues["sw1"];
var startDate = p.fieldValues["strtDate"];
startDate = new Date(startDate)
var endDate = p.fieldValues["endDate"];
endDate = new Date(endDate);
endDate = new Date(endDate);
if (qTags.trim().length==0) {qTags=[]} else {qTags=qTags.split(",")}
if (oTags.trim().length==0) {oTags=[]} else {oTags=oTags.split(",")}
if (sortBy) {sortBy="created"} else {sortBy="modified"}
startDate.setHours(0, 0, 1)
endDate.setHours(23, 59, 59)
//
if (p.buttonPressed == "Consolidate drafts") {
//
//
  drArr = Draft.query("", locat,qTags, oTags,sortBy, sortTime, false);
//found every draft & sorted by modified/created and time ordered
//
  var outArr=[]; // define empty results array
  tx = '';
  strt = startDate.getTime(); //number(msecs post 1970)
  endd = endDate.getTime() //number(msecs post 1970)
  //? msec conversion gives a SLIGHT speed benefit over library comparisons
  for (let n=0;n<drArr.length;n++) {
    if (sortBy=="modified") {t = drArr[n].modifiedAt.getTime();}
    if (sortBy=="created")  {t = drArr[n].createdAt.getTime();}
    if ((t>=strt)&&(t<=endd)) {outArr.push(drArr[n]);}
   }
//
//
//
//
// BUILD THE FOUND DRAFTS INTO ONE COMBINED NOTE
// 1st, set a suitable filename and a first line for the output body
  startDate = strftime(startDate,"%y-%m-%d %a"); // for writing out purposes
  endDate  = strftime(endDate,"%a %y-%m-%d");
  let txtInsert = " daily Drafts", tExt= ".md"; // change as desired, within "...";
  if (startDate==endDate) {     // set filenames depending on days'  matching
    targ = endDate + txtInsert + tExt;
    tnote ="consolidated "+ outArr.length + " Drafts found for "+startDate; // 1st line txt
    } else {
    targ = startDate + "--" + endDate + txtInsert + tExt;
    tnote="consolidated "+outArr.length+" Draft(s) found between "+startDate+" and "+endDate; 
    }
// that gives date-sortable titles 
// "2022-08-15 daily Drafts.md" or "2022-08-15--2022-08-16 daily Drafts.md"  
// now set a suitbale title and a first line for the output body
// construct the rest of the body
  for (let t of outArr) {
     tnote=tnote + divider + strftime(t.modifiedAt,"%a %y-%m-%d %r")+ "\n" + t.content; 
// builds output by one draft content at a time
     }
//
// NOW OUTPUT, looping through found drafts, 
//
// the next target sets are output, disable any SET OF 3 LINES you might want inactive by adding the double slash(//-- comment) to the front of each (or remove)
// you may change any of the wording (within quotes) 
// set an appropriate filename for file systems
// to write to a new draft, uncomment (remove '//':
//  d = new Draft();
//  d.content = tnote;
//  d.update();
//
// to write to the any cloud or local file system Drafts iCloud directory
//leave the next three lines to write to Drafts iCloud 
  fm = FileManager.createCloud();
  fm.createDirectory("Drafts By Day","/");
  t = fm.writeString("/Drafts By Day/"+targ,tnote);
//
// leave the next three lines to write to a Bookmark (if one not set, you can set it as this runs)
//  let bookmark = Bookmark.findOrCreate("DraftsByDay");
//  fm = FileManager.createForBookmark(bookmark);
//  t = fm.writeString(targ,tnote);
// end of this script
}  // end of if button pressed
```

Tags:
  documentation, drafts, js, meta, reference, simplenote, snippets