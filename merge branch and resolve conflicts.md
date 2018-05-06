<code><-- add branch to remote (server: origin, branch: issue52) --></code><br>
<strong>$ git push --set-upstream origin issue52</strong></br>

<code><-- merge branchs (current branch master, we wanna merge to issue52) --></code><br>
<strong>$ git merge issue52</strong></br>

<code><-- you need install merge tool to use when conflicting happen (ex: install diffmerge) --></code><br>
<strong>https://sourcegear.com/diffmerge/downloads.php</strong></br>

<code><-- config merge tool editor --></code><br>
<strong>$ git config --global merge.tool diffmerge</strong></br>
<strong>$ git config --global mergetool.diffmerge.cmd "sgdm --merge --result=\$MERGED \$LOCAL \$BASE \$REMOTE"</strong></br>
<strong>$ git config --global mergetool.diffmerge.trustExitCode true</strong></br>
<strong>$ git config --global mergetool.keepBackup false</strong></br>
<strong>$ git config --global diff.tool diffmerge</strong></br>
<strong>$ git config --global difftool.diffmerge.cmd "sgdm \$LOCAL \$REMOTE"</strong></br>

<code><-- list available merge tools --></code><br>
<strong>$ git config --global merge.tool</strong></br>
