# manifest

安装工具所需工具：
step1:
    Download repo script; (curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo;chmod +x ~/bin/repo)

step2：
    更改repo中的下载路径为国内清华源
        vim ~/bin/repo;   REPO_URL = 'https://mirrors.tuna.tsinghua.edu.cn/git/git-repo'
 
 下载程序：
    1.下载空的框架代码
        a.下载代码信息文件
            repo init -u git@github.com:msrLi/lhb_mainfest.git -m create_empty.xml
        b.同步代码
            repo sync [-j8] 
