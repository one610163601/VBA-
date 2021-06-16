# 上传文件到github的步骤

1. ## 打开git，直接找到项目然后右键`Git Bash Here`

2. ### 通过`git init`命令把这个项目变成一个Git可以管理的仓库

3. ### 第三步：用`git add`命令告诉Git，把项目下的文件添加到仓库

4. ### 用`git commit`命令告诉Git

   把文件提交到仓库,`-m`后面输入的是本次提交的说明，可以输入任意内容，当然最好是有意义的，这样你就能从历史记录里方便地找到改动记录。

   `git commit`命令执行成功后会告诉你，`1 file changed`：1个文件被改动（我们新添加的readme.txt文件）；`1 insertions`：插入了1行内容（test.txt有两行内容）。

   

   ![img](https://img2018.cnblogs.com/blog/1646268/201907/1646268-20190717160805915-782318854.png)

   如果出现以下内容则需要输入自己的账号和邮箱

   按照上面给的代码输入`nane`和`email`后再次执行`git commit`命令。

   

5. ###   输入`git remote add origin 自己仓库地址`将本地仓库关联到GitHub上，然后输入`git push -u origin master`将代码上传到GitHub上。

   执行完后，如果没有异常，会等待几秒，然后跳出一个让你输入Username和Password 的窗口，你只要输人github的登录账号和密码就行了，好了上你的GitHub上看看项目有没有传上去吧。
   
   

 6. ### 更新项目

    当以后需要更新项目的时候有四步需要走
    第一步：执行`git pull`命令将GitHub上的代码当下来合并代码，防止提交新代码的时候起冲突
    第二步：执行`git add`命令将代码添加到仓库
    第三步：执行`git commit`命令将代码提交到仓库
    第四步：执行`git push`命令将代码提交到GitHub
