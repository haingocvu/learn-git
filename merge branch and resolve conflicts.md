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

<code><-- merging 2 branchs can lead to conflict. we need to open diffmerge to resolve it by below command --></code><br>
<strong>$ git mergetool</strong></br>

<code><-- after merging, we confirm by save and exit diffmerge. then, we must to use commit to complete the merging --></code><br>
<strong>$ git commit -m "resolve conflicts"</strong></br>
