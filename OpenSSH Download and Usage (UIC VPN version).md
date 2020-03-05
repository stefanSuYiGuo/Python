# The usage of OpenSSH
---
*Author 苏义国 Stefan*
> Recently, we are supposed to use ***UICVPN*** to connect with *Jupyterhub*. But there is a desperate sentence that **For Windows users, open PowerShell if you are Window 1018 03 or newer, else you should use other ssh tools.** For me, unfortunately I am an outlier. So with teacher's suggestion, I focus on other ssh tool called OpenSSH. Here is some tips you may need.

## Tips for user of OpenSSH
1. First, you should install OpenSSH software. But you cannot install it from [official website](https://www.openssh.com/ "OpenSSH Official Website") directly, because it's hard to find the download file. If you try to search "OpenSSH download for Windows", you will get an zip file, including plenty of .nsi files, which are absolutely inconvenient. For user-friendly, I provide an official website with an executable .exe file. Click [here](https://www.mls-software.com/opensshd.html "OpenSSH executable download").
2. Next, click .exe file to start your download. ![](https://github.com/stefanSuYiGuo/ImageRepository/blob/master/OpenSSH_download_and_Usage_1.png)
3. And then, follow the graphical instructions to install OpenSSH.
    ![](https://github.com/stefanSuYiGuo/ImageRepository/blob/master/OpenSSH_download_and_Usage_2.png)
    ![](https://github.com/stefanSuYiGuo/ImageRepository/blob/master/OpenSSH_download_and_Usage_3.png)
    + remember: unclick "Server" Option
    ![](https://github.com/stefanSuYiGuo/ImageRepository/blob/master/OpenSSH_download_and_Usage_4.png)
    ![](https://github.com/stefanSuYiGuo/ImageRepository/blob/master/OpenSSH_download_and_Usage_5.png)
    ![](https://github.com/stefanSuYiGuo/ImageRepository/blob/master/OpenSSH_download_and_Usage_6.png)
4. Until now, you have installed OpenSSH successfully. Next, press `win + R` and input `cmd` to run Command Prompt as ***administrator***
5. Now, you are going to work on the connection. Input `ssh -N -L localhost:8888:localhost:8080 ws1830026101@172.16.240.253` (**Remember: replace to your own student ID**) ![](https://github.com/stefanSuYiGuo/ImageRepository/blob/master/OpenSSH_download_and_Usage_7.png)
6. For the fist connection, you will be asked to keep connection or not. Just input `yes`. ![](https://github.com/stefanSuYiGuo/ImageRepository/blob/master/OpenSSH_download_and_Usage_8.png)
7. Input `ssh -N -L localhost:8888:localhost:8080 ws1830026101@172.16.240.253` again and enter the initial password 000000. ![](https://github.com/stefanSuYiGuo/ImageRepository/blob/master/OpenSSH_download_and_Usage_9.png)
8. And then change your password as soon as possible. Like this: ![](https://github.com/stefanSuYiGuo/ImageRepository/blob/master/OpenSSH_download_and_Usage_12.png)
9. Next, visulize to you browser. In the address bar, input `localhost:8888` and press *Enter*. You will get the following: ![](https://github.com/stefanSuYiGuo/ImageRepository/blob/master/OpenSSH_download_and_Usage_10.png)
10. Here is a successful page. ![](https://github.com/stefanSuYiGuo/ImageRepository/blob/master/OpenSSH_download_and_Usage_11.png)
11. Finally, you can follow other instructions provide in this [link](https://ispace.uic.edu.hk/pluginfile.php/154525/mod_page/content/2/Jupyterhub_readme.pdf?time=1583392406516 "An introduction to our Jupyter Hub")

#### Thank you for your reading! Hopefully, it can help you.
