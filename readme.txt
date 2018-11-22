Git is a version control system.
Git is free softwore.
to be or not to be ,that is a question.
//查看分支 git branch
//创建分支  git branch <name>
//切换分支  git checkout <name>
//创建+切换分支 git checkout -b dev
//合并某分支到当前分支 git merge <name>
//删除分支 git branch -d dev

//master和dev不同分支之间解决冲突

go on the way

标签：
①打标签 git tag <标签名>
②打带备注的标签 git tag -a <标签名> -m <备注>
③查看所有标签 git tag
④查看某一个标签 git show <标签名>

指定commit id打tag
git tag -a <标签名> -m <备注>  <commit id>

删除标签：
git tag -d <标签名>

因为创建的标签都只存储在本地，不会自动推送到远程。所以，打错的标签可以在本地安全删除。


推送标签到远程：
git push origin <标签名>

将本地未推送到远程的标签一次性推送到远程：
git push origin --tags

删除远程标签：
①删除本地标签：git tag -d <标签名>
②删除远程：git push origin :refs/tags/<标签名>
