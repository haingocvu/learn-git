<code><-- listing the availabel tags --></code><br>
<strong>$ git tag</strong></br>

<code><-- searching for tags with a particular pattern --></code><br>
<strong>$ git tag -l "v1.9.2*"</strong></br>

<code><-- creating an annotated tag (recommended) - tagging the last commit--></code><br>
<strong>$ git tag -a v1.0 -m "release 1.0"</strong></br>

<code><-- git show tag info --></code><br>
<strong>$ git show v1.0</strong></br>

<code><-- creating lightweight tag (not recommended) --></code><br>
<strong>$ git tag v1.0</strong></br>

<code><-- pretty log --></code><br>
<strong>$ git log --pretty=oneline</strong></br>

<code><-- tagging a specific commit (ex: commit id = 815e6954e2d65d8006675fcfeb579aaf8b1ae1c7) --></code><br>
<strong>$ git tag -a v0.1 815e6954e2d65d8006675fcfeb579aaf8b1ae1c7 -m "release v0.1. first tag"</strong></br>

<code><-- push a single tag to server (ex: servername is origin, tag name is v0.1) --></code><br>
<strong>$ git push origin v0.1</strong></br>

<code><-- push all tags to server (ex: servername is origin) --></code><br>
<strong>$ git push --tags</strong></br>

<code><-- checking out tag as new branch (git checkout -b [branchname] [tagname])--></code><br>
<strong>$ git checkout -b version1.0 v1.0</strong></br>

<code><-- deleting a tag on local --></code><br>
<strong>$ git tag -d v1.1</strong></br>

<code><-- listing tags on remote --></code><br>
<strong>$ git ls-remote --tags</strong></br>

<code><-- deleting a tag on remote (ex: remote name: origin, tag name: v1.1)--></code><br>
<strong>$ git push origin --delete v1.1</strong></br>
