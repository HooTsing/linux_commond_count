### clone项目
* clone项目到本地     
`git clone <http://yourGitAddress.git>`

### 查看状态
* 查看工作区状态     
`git status`

### 回滚

*  硬回滚       
`git reset --hard commit_id`
 
* 软回滚    
`git reset --soft commit_id`


### 存储

* 将暂存区文件存入临时存储(请在切换分支之前提交您的更改或隐藏它们)      
`git stash`                  

* 暂存后切换分支    
`git checkout [branch]`

* 查看储存的修改    
`git stash list`

* 恢复后手动stash    
`git stash apply`

* 清除stash     
 `git stash drop`

* 全部清除stash     
`git stash clear`

* 多个stash时,恢复指定stash需加上id     
`git stash apply stash@{id}` 

* 将最顶部的stash拉出    
`git stash pop`

* 和apply同理      
`git stash pop stash@{id}`


### 子模块

`.gitmodules文件` **该配置文件保存了项目 URL 与已经拉取的本地目录之间的映射**

* 子模块文件初始化     
`git submodule init` 

* 拉取子模块      
`git submodule update`

* 拉取子模块（合并上面两步）     
`git submodule update --init --recursive`

[子模块文档](https://git-scm.com/book/zh/v2/Git-%E5%B7%A5%E5%85%B7-%E5%AD%90%E6%A8%A1%E5%9D%97)

### 添加文件

* 添加文件       
`git add filename`

* 按模块添加文件      
`git add -p` 

### 分支

* 查看分支关联    
`git branch -vv`  

* 删除分支      
`git branch -d <branch>`

* 查看远端和本地所有分支     
`git branch -a`

### 合并

* 合并多条commit到一起  
`git merge --squash another`

### git checkout

* 切换分支    
`git checkout <branch_name>`

* 放弃指定分支branch_name对指定文件file_name的修改     
`git checkout <branch_name> <file_name>`

### 删除

* 删除服务器远端的分支      
`git push origin –delete <branch>`

* 删除本地已合并分支    
`git branch –d <branch>` 

* 删除本地未合并的分支         
`git branch –D <branch>` 
