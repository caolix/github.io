# 在Github上建立自己的个人博客网站详细教程

## 创建仓库

登录自己的GitHub账户，通过“New repository”创建自己的仓库。设置自己的访问路径，具体看配置流程。

## 创建本地仓库

添加本地id_rsa.pub到github，下载远程仓库到本地，并配置如下信息

```
git config --global user.name “你的Github用户名”
git config --global user.email “你的Github邮箱地址”
```

## 使用Jekyll创建博客模板

1. 去[Jekyll Themes](http://jekyllthemes.org/)下载一个自己喜欢的模板
2. 按照之前的步骤把下载好的模板上传到自己的Github仓库中
3. 在_posts文件夹中放入自己写好的博客,文件名必须是日期-标题名,例如:2016-10-25-我的第一篇博客
4. 上传博客到Github中即可访问自己的博客

## demo

```
https://starry99.github.io/catbook
```

## Setup

```sh
$ git clone https://github.com/starry99/catbook
$ jekyll serve

# Now you can start customization!
```

## Make it yours

If you want to create a new category, you need to create `*name*.html` in the `categories` folder. And add the following content:
```html
---
layout: page
type: *name*
---

{% include archive.html %}
```
Then the number of pages in the category will be displayed.

## License

[MIT License](https://opensource.org/licenses/MIT)
