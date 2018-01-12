HTTPS -第一次初始化+提交数据
- git init
- git config user.name zgf
- git config user.email 894453713@qq.com
- git remote add origin https://github.com/soar26/study.git
- git push -u origin master

SSH -第一次初始化+初始化数据
- git init
- git config user.name zgf
- git config user.email 894453713@qq.com
- git remote add origin git@github.com:soar26/study.git
- git push -u origin master

复制
 git clone https://github.com/soar26/study.git
 git clone git@github.com:soar26/study.git

生成密钥
 ssh-keygen

问题1、从复制过来的仓储进行操作?
在初始化的文件夹下进行如下操作（已经有私钥）
1.git clone git@github.com:soar26/study.git
2.cd study
3.修改信息
4.git add 
  git commit -m "..."
5.git push
问题2、本地仓储和远程不同步，如何办?
 git pull --rebase origin master
问题3，分支？
git branch
git branch dev_test
git checkout dev_test
git checkout master
git merge --no-ff dev_test
问题4，冲突？
git diff
问题5，回退？
git log
git reset --hard XXX对应版本号
问题6，帮助？
git help
问题7， egit ssh提交 https提交？
egit https提交不需要公钥和私钥
egit ssh提交需要公钥和私钥
问题8，egit ssh配置?
ssh2:Generate RSA Key->Export Via SFTP(git@github.com)->Load Existing Key->save->Apply close
git:(1)Committing 第一项去掉对勾；（2）Configuration,User Setting添加用户名和邮箱
