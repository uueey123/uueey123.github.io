---
layout: page
title:  "composer与laravel框架架设"
subtitle: "composer+laravel"
date: 2020-10-13；
categories: ['框架基础']
---

> 当下载并安装完毕小皮之后，开始搭设composer与laravel框架

## Composer   
- 在c盘以管理员身份打开Powershell，执行以下代码 
    - php -r "copy('https://install.phpcomposer.com/installer', 'composer-setup.php');"
        - 在上方网站中下载文件，并且重命名为composer-setup.php这个文件
        - 整行代码的意思为php，-r（解析后方链接的文件）,copy（复制并重命名为后面的名字composer-setup.php）

    - composer --version
        - 等下载完毕之后检查是否下载成功并检查版本

## 阿里云镜像源
- 当comperser下载完毕后，执行以下代码
    - composer config -g repo.packagist composer https://mirrors.aliyun.com/composer/
        - 把composer的更新链接替换成阿里云的镜像链接
    - composer self-update
        - 更新composer至最新版本


## Laravel
- 当composer下载并更新完毕后，执行以下代码    
    - composer create-project --prefer-dist laravel/laravel blog "5.5.*"
        - 以composer下载laraverl并且在目标文件夹创建一个叫做blog的文件夹


---