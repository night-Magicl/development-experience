                                            首次创建项目，向master推送代码，有两种方式
	前提：在创建仓库前先部署好ssh
	1：通过Sourcetree
		在GitHub上创建一个仓库，README.md文件需要
		然后通过Sourcetree拉取master代码，然后将项目文件移动到改根目录下，推送到远程
	2：通过gitbash，参考：https://blog.csdn.net/u010420283/article/details/84791830
		echo "# HelloWorld" >> README.md
		git init
		git add README.md （add后跟推送文件，（git add .） 就是推送该目录下所有文件）
		git commit -m "first commit"
		git remote add origin https://github.com/Briwisdom/HelloWorld.git（后面跟的GitHub地址也可以是ssh地址）
		git push -u origin master
	
                                              Sourcetree通过ssh拉取代码
	参考：https://segmentfault.com/q/1010000014540808
	使用git bash命令工具创建ssh密钥（cd ~/ .ssh），然后把id_rsa。pub文件内的公钥复制到仓库的ssh-key中
	然后通过工具>选项->添加ssh密钥添加了id_rsa文件,选项内的ssh客户端选OpenSSH
                                              
                                              git bash 常用命令
	git add .   (选择提交文件，add后可跟具体文件名，. 是所有文件）
	git commit -m ''
	git push
