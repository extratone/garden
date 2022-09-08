---
{"dg-publish":true,"permalink":"/snippets/ia-download-md/","dgHomeLink":true,"dgPassFrontmatter":false}
---

ia-download.md
# Downloading and Syncing Archive.org Collections

Following are instructions on how to use the Internet Archive command-line tool, "ia", to download a collection from Archive.org and keep it synced.
The only requirements are that you have Python 2 installed on a Unix-like operating system (i.e. Mac OS X, Linux).


## Downloading and Configuring the Ia Command-Line Tool

1. Download the latest binary of the `ia` command-line tool:

    `$ curl -L https://archive.org/download/ia-pex/ia > ia`

2. Make the binary executable:

    `$ chmod +x ia`

3. Configure `ia` with your Archive.org credentials (This step can be skipped if you are downloading from a public collection):

    `$ ./ia configure`

## Downloading and Syncing an Archive.org Collection

The following command will download all files for all items in the https://archive.org/details/ArchiveIt-Partner-168 collection.

The `--checksum` option will allow you to easily resume your download if something goes wrong, or to keep your local collection in sync with the collection on Archive.org.
When the `--checksum` option is included in your command, `ia` will skip over any files that have already been downloaded (granted the md5 checkusm of the local file matches the md5 of the file on Archive.org).

The `--log` option will generate a log file in the directory from which you run the command, called `internetarchive.log`.
For more details and options, run `ia download --help`.

```
$ ./ia download --search 'collection:ArchiveIt-Partner-168' --checksum --log
```

To keep your local collection in sync with the collection on Archive.org, the above command can simply be rerun.

Tags:
  snippets