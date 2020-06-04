# 博客地址：
### strivefar.github.io

    


# 博文发送流程
### 1. 在根目录下执行`hugo new project/post/新文章文件夹/XXX.md` 后自动创建如下


	    # Documentation: https://sourcethemes.com/academic/docs/managing-content/
	    title: "XXX"
	    subtitle: ""
	    summary: ""
	    authors: []
	    tags: []
	    categories: []
	    date: 2020-06-04T13:55:02+08:00
	    lastmod: 2020-06-04T13:55:02+08:00
	    featured: false
	    draft: false
	    
	    # Featured image
	    # To use, add an image named `featured.jpg/png` to your page's folder.
	    # Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
	    image:
	      caption: ""
	      focal_point: ""
	      preview_only: false
	    
	    # Projects (optional).
	    #   Associate this post with one or more of your projects.
	    #   Simply enter your project's folder or file name without extension.
	    #   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
	    #   Otherwise, set `projects = []`.
	    projects: []



#### <1>其中可以选择的有：
    
	    title: '文章名字动态编译和静态编译——制作动态库和静态库'
	    subtitle: 如有问题，欢迎各位批评指正。 :rocket:'
	    summary: 
	    authors:
	    - youngfar
	    tags:
		#可选的标签有
	    - *
	    - 嵌入式
	    - linux
	    - gcc
	    - C
	    - 数据结构与算法
	    - STM32
	    - IMX6ULL
	    - 待添加
	    categories:
		#可选的种类
	    - gcc编译调试问题
	    - 嵌入式linux学习笔记
	    - Git & Github
	    - C语言学习
	    - STM32
	    - 天猫精灵IOT平台
	    - 待添加


#### <2>文章配图可以使用
	https://unsplash.com

**这个网站的需要下载到本地，和文章XXX放在同一目录**

	project/post/新文章文件夹/

**图片的命名必须为**
	
	featured.jpg/png
**( To use, add an image named `featured.jpg/png` to your page's folder.)**

#### <3>关于博文的图片，
保险起见，使用github存储 每篇文章的图片均在
`static/img/`
下建立一个文件夹

引用时如下：

##### 注意是斜杠（问号键），不是反斜杠

	![wechat](/img/conta/wechat.jpg)

### 2.编辑好博文内容后，退出到根目录blog   

执行以下命令将博客部署到远端

	hugo --theme=academic --baseUrl="https://strivefar.github.io/" --buildDrafts

### 3.执行后生成public，进入public目录，这是最终要推送的目录

	cd public

### 4.然后 依次执行如下命令，上传到github,至此博客文章更新完成

    git add --all
    
    git commit . -m"add new XXX."
    
    git push origin master
