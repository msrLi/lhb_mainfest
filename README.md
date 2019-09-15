# manifest

## 安装工具所需工具：
* step1:
   * Download repo script; (curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo;chmod +x ~/bin/repo)

* step2：
   * 更改repo中的下载路径为国内清华源
   * vim ~/bin/repo;   REPO_URL = 'https://mirrors.tuna.tsinghua.edu.cn/git/git-repo'
 
### 下载程序：
* 1.下载空的框架代码
* a.下载代码信息文件
    repo init -u git@github.com:msrLi/lhb_mainfest.git -m [ create_empty.xml   or   ejd_thread.xml or neptunium.xml ] 
* b.同步代码
    repo sync [-j8] 



## 配置文件说明：

* create_empty.xml 
   * `--> target    [target_base | git@github.com:msrLi/target_base.git]`
   * `              target 基础框架代码`
   * `--> makerules [utils-tools | git@github.com:msrLi/utils-tools.git]`
   * `         编译脚本和工具脚本文件`
* ejd_thread.xml

* neptunium.xml
     * ` 下载同步  repo init -u git@github.com:msrLi/lhb_mainfest.git -m neptunium.xml ；  repo sync`
     * `               or repo init -u https://github.com:msrLi/lhb_mainfest.git -m neptunium.xml ；  repo sync`
     * `--> target    [target_base | git@github.com:msrLi/neptunium.git]`
     * `              target 基础框架代码`
     * `--> makerules [utils-tools | git@github.com:msrLi/utils-tools.git]`
     * `         编译脚本和工具脚本文件`
