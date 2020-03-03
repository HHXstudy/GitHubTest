# Git学习笔记

## Git结构
工作区,暂存区,版本库
工作区（WORKING DIRECTORY）: 直接编辑文件的地方，肉眼可见直接操作；

暂存区（STAGIN AREA）：数据（快照）暂时存放的地方；

版本库（GIT DIRECTORT(RESPOSITORY)）：存放已经提交的数据，push 的时候，就是把这个区的数据 push 到远程git仓库了。

## Git指令

git init 初始化git项目

git status 查看项目状态

git add [filename] 就是将工作区的修改缓存在暂存区

git commit [filename] 就是将暂存区的数据快照提交到本地库

     -m "提交注释"

git config 项目相关配置信息

    user.name xxx 当前项目用户的名称

    user.email xxx 当前项目用户的邮件

    --global 全局设置

git log 查看项目历史记录
    多屏显示下的控制方式:空格向下翻页，b向上翻页，q推出
    --pretty=oneline 将每次修改按行简洁的显示
    --oneline 将每次修改按行更简洁的显示(哈希值显示前7位)

git reflog
    HEAD@{移动到目标版本所需步数}
    