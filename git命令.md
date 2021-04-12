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
    git log --autor='zhangyuan'             查找某一个用户的操作记录

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
    git mv demo.html home（把demo.html文件夹移动到home文件夹中）
    git mv demo.html home/home.html (把demo.html文件夹移动到home文件夹下并且修改为home.html)

6、查看某一个文件的修改记录
    git log -p demo.html

7、操作失误的情况下如何实现一件还原
    

