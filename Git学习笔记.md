---
日期：11.9
作者：吴思雨
分类：Git
---

[Git学习笔记](#Git学习笔记)

# Git学习笔记

(*说明：由本人在小红书上搜索出的Git命令总结和运用AI工具豆包进行第一次实操总结而成。*)

## 常用命令语句总结

| 命令                                                         | 说明             |
| ------------------------------------------------------------ | ---------------- |
| git config --list                                            | 查看已配置信息   |
| git config --global user.name "your name"/user.email "your email" | 设置基础信息     |
| git init 仓库地址                                            | 初始化本地仓库   |
| git status                                                   | 查看文件状态     |
| git add 文件名                                               | 暂存文件         |
| git commit -m "提交说明"                                     | 提交到本地仓库   |
| git push                                                     | 推送到远程仓库   |
| git pull                                                     | 拉取远程最新代码 |

## 远程提交文档到Github仓库

1. 在本地创建文件；
2. 用git进入文件所在文件夹（e.g.cd desktop"）；
3. 初始化本地git仓库：git init；
4. 把文件加入暂存区：git add 文件名；
5. 把文件转移到本地仓库：git commit -m "备注说明"；
6. 关联Github远程仓库：git remote add origin 网址（origin是远程仓库的别名）；
7. 推送文件到远程仓库：git push -u origin main/master(默认仓库分支)（-u是记住关联，下次可直接输入git push）；
8. 进入合并提交的备注编辑页面：1. 按‘i’键，待底部出现--INSERT--；2.输入说明；3.按Esc键，--INSERT--消失；4.输入":wq";5.按回车键。
9. github登录验证授权，完成提交；

## 易错点

1. 在7.中若是新仓库首次推送需要先输入：git pull origin master --allow-unrelated-histories在输入7.内容
2. 网络可能会报错，不用在意，等待即可；
3. 其他不常见错误见[第二阶段问题与解决][1]。



[1]:https://github.com/llf915915/wsy-learning-world/blob/main/%E9%97%AE%E9%A2%98%E8%A7%A3%E5%86%B3.md