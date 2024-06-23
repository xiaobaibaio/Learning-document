### 将项目保存到GitHub

git常规指令

```bash
#git初始化
git init
#查看文件是否被追踪
git status
#将项目所有文件保存到git暂存区
git add .
#提交git暂存区
git commit -m "<名字>"
#查看提交历史（--oneline表示简化记录）
git log --oneline
#比较记录
git diff <id编号> -- 文件名称
#还原记录
git checkout <id编号> -- 文件名
#将本地变更自动推送到GitHub
git push
#推送本地的 main 分支到远程仓库
git push origin main
#查看分支
git branch
#新建分支
git branch <名字>
#切换到新分支
git switch <名字>
```

项目保存到GitHub

```bash
git -c http.sslVerify=false clone https://github.com/xiaobaibaio/sky-take-out.git
```

