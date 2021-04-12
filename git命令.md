一、
    git init                代码初始化
    git add .               提交到缓存区
    git commit -m           提交
    git status              查看修改的状态
    git pull                更新

    git remote add origin https://github.com/Jerryzhangyuan.git     远程连接


二、
1、查找所有的操作记录
    git log                                 查找所有的记录
    git log --author='zhangyuan'             查找某一个用户的操作记录

2、配置用户名和邮箱
    git config --global user.name 'zhangyuan'               配置用户名
    git config --global user.email '14177112622@qq.com'     配置邮箱
    git config --global --list                              查看配置的用户名跟邮箱

3、想要删除项目中文件的时候如何操作
    手动删除
    命令行删除：git rm demo.html(直接删除成功)

4、想要给文件重命名时如何操作
    手动修改
    命令行修改：git mv demo.html index.html (把demo.html文件修改为index.html)

5、移动文件到其他的位置如何操作
    git mv demo.html home(把demo.html文件夹移动到home文件夹中)
    git mv demo.html home/home.html (把demo.html文件夹移动到home文件夹下并且修改为home.html)

6、查看某一个文件的修改记录
    git log -p demo.html

7、操作失误的情况下如何实现一键还原
    (1)、还没有添加到暂存区，只是误改动了
        git checkout -- demo.html
    (2)、已经提交到暂存区
        git reset HEAD demo.html
        git checkout -- demo.html
    (3)、代码已经commit提交了
        A、还原到上一个版本(回到上几个版本，HEAD后面就加几个^)
            git reset --hard "HEAD^"
        B、直接还原到上某个版本(版本id根据git log查看)
            git reset --hard 版本id

8、分支的创建、删除、切换
    (1)、创建dev分支：git branch dev
    (2)、删除dev分支：git branch -d dev
    (3)、切换到test分支：git checkout test
    (4)、创建adm分支，并且切换到该分支：git checkout -b adm
    备注：在当前分支时，当前分支不可以删除。在分支commit了代码，改分支不可以删除，如果要删除，则强制删除(git branch -D test)



