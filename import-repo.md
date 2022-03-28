# 使用Git上传本地项目到GitHub仓库
  1、单机右上角 + 号，选择New repository创建新仓库。
  
  ![图1](https://user-images.githubusercontent.com/82021888/160408408-04ce66c7-b8b9-4c71-af36-d46f6365ffdf.png)
  ![图2](https://user-images.githubusercontent.com/82021888/160408659-9b31c760-c626-491f-bbff-3eade360c79d.png)
  
  2、打开新建的仓库，点Code复制该仓库地址。备用。
  
  ![图3](https://user-images.githubusercontent.com/82021888/160409462-ba481565-8b3e-4202-b52d-2f9f1d05b14b.png)
  
  3、到本地项目更目录下，右键Git Bash Here，在弹出的命令框中输入以下命令。
  
    git init （初始化Git）
    git add . (将所有项目文件添加到缓存区)
    git commit -m "备注信息" （增加备注）
    git remote add origin https://github.com/Marous-LXB/STC8H-8A.git （关联GitHub上的仓库地址）
    git push -u origin master （将缓存区内容上传到GitHub仓库，弹出窗口后输入GitHub用户名密码确认）
    
  ![图4](https://user-images.githubusercontent.com/82021888/160412020-879e76ed-8c2e-43b4-878d-55fef582d873.png)
  ![图5](https://user-images.githubusercontent.com/82021888/160412792-b2205d54-bc7a-4aac-93fd-dc9525382e07.png)
  ![图6](https://user-images.githubusercontent.com/82021888/160412877-fab994f2-4493-4d80-9503-9b878530d988.png)
  
  4、等待上传完成，之后就可以在GitHub上看到上传的内容了。
  
  ![图7](https://user-images.githubusercontent.com/82021888/160413314-0d2fb341-57d7-4123-bb3c-32fa8e5538d8.png)

  

