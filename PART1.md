# Welcome to use MarkDown  
## 中文输入法：option->Text UTF-8 

workspace **-add-** index **-commit-** repository **-checkout-**     

## section 0 GIT提交文件环境配置：**在~/目录下.gitconfig;**    
  - git config --list(配置相关的参数)    
  - git config --global user.name "BurgessH"  
  - git config --global user.name "20428770246@qq.com"  
  
## Section 1  
  - git bash命令上     
    - git init (初始化本地仓库)     
    - git add README.md(指定文件到暂存区)   
    - git commit -m "Message" 
    - git commit -a -m （已有历史版本的提交信息,直接从暂存区提交到仓库）   
    - git status (查看文件信息)  
    - git log/--oneline（查看提交信息）  
    - git show 哈希值  
    - git rm    
    - git mv   
    
  - git bash命令下  
    - git remote add Origin https://github.com/BurgessH/Demo(关联本地仓库和远程仓库)  
    - git remote -v 
    - git push origin master  本地仓库推送到服务器上  
    - git pull origin master   
    - git clone https://github.com/BurgessH/demp  

# Git配置
## ignore
  - 忽略HB创建的文件；
  - git add -f(强制添加.gitignore忽略文件)
  - git reset HEAD
  - git check-ignore -v .project(查看.gitignore策略生效行号)
  
## Github Mode
 - cerat repository 添加.gitignore的类型文件；
 
## 换行  
- 提交时转换为LF，检出时转换为CRLF，默认设置不用修改，git是Linux配置；  
  - git config --global core.autocrlf true   
  
- 允许提交包含混合换行符的文件   
  - git config --global core.safecrlf false  
  
  - **CR:** carriage return回车，光标到首行，‘\r’=return   
  - **LF:** line feed换行，光标下移一行，‘\n’=newline  
    - **linux: line feed \n**  
    - **windows: line feed \r\n**  
    - **MAC OS: line feed \r**  
    
## 别名
### 以图形的方式打印Git提交日志
  - git log --pretty=format:'%h %ad | %s%d [%an]' --graph --date=short
  
### 设置别名
	- git config --global alias.ci commit	
	
## 凭证
  - git config --global credential.helper wincred

## Git命令
 - git
 - git blame
 - git ckean -x -f (删掉.gitconfig中.project文件)
 - git st -sb(短信息的方式显示)
 - git add .
 - git add -p (一个文件多个提交:分块提交)
 - git reset HEAD 
 
 ## 查看深入信息
 - git status -sb 
  
![diff](23.png)

 ## 查看某个提交信息  
 - git show HEAD^前一个提交； ~前两个；
 
 ## 查看提交历史  
 - git log Part3.md  
 - git show  35e67a0  
 - git log --grep add(筛选信息)  
 - git hi -10 
 - git -am "massage"(已经有提交记录)  
 
## 版本比较
 - git diff   
 
## 规范化massage  
  - type (scope): subject  
    - type:  
      - feat:新功能  
      - fix: 修改bug  
      - docs:文档  
   		- style: 格式  
   		- refactor: 重构   
   		- test:  
   		- chore:  

 - body  
 - footer   

 - Ubuntu下的安装方法:  

   - sudo add-apt-repository ppa:notepadqq-team/notepadqq   

   - sudo apt-get update  

   - sudo apt-get install notepadqq  


 - Ubuntu下的卸载方法:  
 
   - sudo apt-get remove notepadqq        
 
   - sudo add-apt-repository --remove ppa:notepadqq-team/notepadqq       
 








