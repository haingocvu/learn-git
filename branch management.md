<code><-- listing the availabel branches --></code><br>
<strong>$ git branch</strong></br>

<code><-- to see the last commit on each branch --></code><br>
<strong>$ git branch -v</strong></br>

<code><-- to see which branches are already merged into the branch you're in. use this command --></code><br>
<strong>$ git branch --merged</strong></br>
  
<code><-- to see all the  branches that contain work you haven't yet merged in. use this command --></code><br>
<strong>$ git branch --no-merged</strong></br>

<code><-- to delete the branch is already merged into the branch you're in. use this command --></code><br>
<strong>$ git branch -d testingbranch</strong></br>
  
  <code><-- to delete the branch is <strong>NOT</strong> merged into the branch you're in. use this command --></code><br>
<strong>$ git branch -D testingbranch</strong></br>
