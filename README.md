# strivefar.github.io


##  ##本地主题生成和预览：

    hugo server


##  ##博文发送流程
1. 每次发博文时，
执行


    	hugo new content/post/新文章文件夹/XXX.md


2. 复制

	**content/post/新文章文件夹** 

	下的内容到

 	**content/project/post/** 

3. 退出到根目录blog ，执行以下命令将博客部署到远端


    	hugo --theme=academic --baseUrl="https://strivefar.github.io/" --buildDrafts

	执行后生成public

4. 进入**public**目录，这是最终要推送的目录

		cd public


5. 然后 依次执行


		git add --all

		git commit . -m"add getting-started."

		git push origin master

6. 关于博文的图片，保险起见，使用github存储
	每篇文章的图片均在**static/img/**下建立一个文件夹

	引用时如下：

		![wechat](/img/conta/wechat.jpg)
