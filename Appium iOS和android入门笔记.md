#Appium IOS和Android入门笔记
1、appium-doctor采用node.js编写，采用npm即可在Terminal中进行安装：npm install appium-doctor -g
安装完毕后，执行appium-doctor命令即可对Appium的环境依赖情况进行检测；指定--ios时只针对iOS环境配置进行检测，指定--android参数时只针对Android环境配置进行检测，若不指定则同时对iOS和Android环境进行检测。例如：appium-doctor --ios
若检测结果通过的话，说明Appium的相关依赖已经准备就绪，可以继续安装Appium