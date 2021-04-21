在windows上使用free surfer

- 安装wsl
  
- 安装ubuntu 18，不要安装20
  
- 按照官网上说明安装需要的库
  - https://surfer.nmr.mgh.harvard.edu/fswiki/WindowsSupport
  - tcsh 可能会提示找不到 解决办法：https://www.reddit.com/r/linux4noobs/comments/dda50d/no_package_named_tsch_and_getting_bintsch_bad/
- linux上安装freesurfer的方法
  - https://surfer.nmr.mgh.harvard.edu/fswiki//FS7_linux
  
  - 按照上述网址centOS7 + tester using sudo+tar.gz的情况安装
  
  - usr/local位置：C:\Users\Administrator\AppData\Local\Packages\CanonicalGroupLimited.Ubuntu18.04onWindows_79rhkp1fndgsc\LocalState\rootfs
  
    或者在C盘中搜索 rootfs



freesurfer short course

https://andysbrainbook.readthedocs.io/en/latest/FreeSurfer/FreeSurfer_Introduction.html



作为MNE的工具开始使用：https://mne.tools/stable/auto_tutorials/source-modeling/plot_background_freesurfer.html

- first steps：
  - 配置freesurfer home和subjects文件夹（里面为若干subject）的位置
  - 之后bash执行$FREESURFER_HOME/SetUpFreeSurfer.sh
  - 遇到没有写入权限的问题，更换sample位置解决 https://www.mail-archive.com/freesurfer@nmr.mgh.harvard.edu/msg65221.html
- 报错：libgomp1 没有找到
  - 解决：sudo apt-get install libgomp1
  - http://webcache.googleusercontent.com/search?q=cache:0CZXUrsS-CoJ:https://andysbrainbook.readthedocs.io/en/latest/FreeSurfer/FS_ShortCourse/FS_02_DownloadInstall.html&hl=zh-CN&gl=us&strip=1&vwsrc=0
- 提示没有授权
  - 前往http://surfer.nmr.mgh.harvard.edu/registration.html进行注册
- 之后可成功recon

