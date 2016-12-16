# MINIST_DBN

这个项目主要是在Python下用DBN对MNIST数据集进行识别分类

#安装环境配置

1. winpython 2.7 安装与环境变量配置

	winpython集成了numpy、scikitlearn、pandas、matplotlib等科学计算需要的环境，对于手动安装各种模块来说，
	winpython更方便。由于该程序使用的关键模块nolearn为0.5b1版，该版本只支持python2，所以使用winpython2.7
		
	1.1 安装
		
	最新版winpython2下载地址：
	https://sourceforge.net/projects/winpython/files/WinPython_2.7/2.7.10.3/
		
	1.2 环境变量配置
		
		将以下路径加入到Path里：
			1 ...\WinPython\scripts
			2 ...\WinPython\python-2.7.10.amd64\Scripts
			

2. MINIST数据集和nolearn的下载与安装

	下载地址：
		https://pan.baidu.com/s/1kULzKJ9			提取码：wanb
		
	2.1	MINIST数据集的存放路径为：
	
		...\WinPython\settings\scikit_learn_data\mldata		
	2.2 nolearn安装方法：
			
		打开CMD控制台
		切换到nolearn文件夹路径：
			cd ...\nolearn-0.5b1
		输入以下内容完成安装：
			python setup.py install
		需要注意的是，安装过程中会出现'build\lib' does not exit，需要手动把nolearn包复制到以下路径:
			...\WinPython\python-2.7.10.amd64\Lib
3. opencv的安装与环境变量配置

	3.1 需要的opencv版本为 2.4.x / 3.x
	
	下载地址：
		http://opencv.org/downloads.html

		在windows下会出现已解压但是硬盘里找不到的情况，这里不要双击打开.exe文件，使用压缩软件打开
	
	3.2 环境变量配置
	
		如果是64位系统，将以下路径加入到Path：
			...\opencv\build\x64\vc11\bin
			
		如果是32位系统，则路径为：
			...\opencv\build\x32\vc11\bin
			
		然后把：
			...\opencv-2.4.13\build\python\2.7\x64\cv2.pyd
		复制到:
			...\WinPython\python-2.7.10.amd64\Lib\site-packages
