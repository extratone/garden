---
{"dg-publish":true,"permalink":"/snippets/update-status-sh/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# update-status.sh

- [update-status.sh](https://gist.github.com/ecstasy2/52dbe5da4a16bb61bb33e4405e5b83fa)
- [WTF](https://davidblue.wtf/drafts/A5D3B194-5461-48CF-93BF-056218011481.html)
- [Things](things:///show?id=CW45XjwiK9duEbJSAb3WM8)


```
https://gist.github.com/ecstasy2/52dbe5da4a16bb61bb33e4405e5b83fa
```

<script src="https://gist.github.com/ecstasy2/52dbe5da4a16bb61bb33e4405e5b83fa.js"></script>

## Bash script to update github commit status


```sh
#!/bin/bash

set -e

# Usage: ./update-status.sh --sha=somesha \
#   --repo=edyn/service-identity \
#   --status=pending \
#   --message="Starting tests" \
#   --context=edyn/e2e \
#   --url=http://something.com
#

STATUS=${STATUS:-"pending"}
REPO_SLUG=${REPO_SLUG:-}
BUILD_URL=${BUILD_URL:-}

for i in "$@"
do
case $i in
    -s=*|--sha=*)
    COMMIT_SHA="${i#*=}"
    shift # past argument=value
    ;;
    -r=*|--repo=*)
    REPO_SLUG="${i#*=}"
    shift # past argument=value
    ;;
    -m=*|--message=*)
    CHECK_MESSAGE="${i#*=}"
    shift # past argument=value
    ;;
    -u=*|--url=*)
    BUILD_URL="${i#*=}"
    shift # past argument=value
    ;;
    --status=*)
    STATUS="${i#*=}"
    shift # past argument=value
    ;;
    -c=*|--context)
    CHECK_CONTEXT="${i#*=}"
    shift # past argument with no value
    ;;
    *)
            # unknown option
    ;;
esac
done

echo "COMMIT_SHA  = ${COMMIT_SHA}"
echo "REPO_SLUG   = ${REPO_SLUG}"
echo "STATUS    = ${STATUS}"
echo "CHECK_CONTEXT    = ${CHECK_CONTEXT}"
echo "BUILD_URL    = ${BUILD_URL}"
echo "CHECK_MESSAGE    = ${CHECK_MESSAGE}"

echo $CHECK_MESSAGE
set -x

curl -u $GITHUB_USER_TOKEN \
 --header "Content-Type: application/json" \
 --data '{"state": "'$STATUS'", "context": "'$CHECK_CONTEXT'", "description": "'"$CHECK_MESSAGE"'", "target_url": "'$BUILD_URL'"}' \
 --request POST \
 https://api.github.com/repos/$REPO_SLUG/statuses/$COMMIT_SHA
```

Tags:
  cli, dev, sh, shell, snippets