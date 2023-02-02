# Blog Admin

> 一个基于 Vue2.0 的博客后台管理项目

## 功能

+ 第三方登录（GitHub、Gitee）
+ 仪表盘
+ 创作平台
  - 系列管理
  - 文章管理
  - 专栏管理
  - 草稿管理
  - 想法管理
  - 读书笔记管理
  - 推荐信息管理
  - 链接信息
+ 微信平台
  - 图文素材库
  - 素材库
  - 自动回复
+ 资源管理
  - 文件管理
  - 图库
+ 系统管理
  - 菜单管理
  - 实体管理
  - 作业管理
  - 用户信息
  - 选项集
  - 系统参数
  - 角色管理

## 启动

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev
```

## 生成

> 注：本项目使用`Github Action`自动发布镜像

手动：

```bash
docker build -f ".\Dockerfile" -t carldu/blog-html-admin:latest .
```

## 部署

快速部署：

```bash
docker run -p 80:80 --name blog-ui -d carldu/blog-html-admin:latest
```

映射`nginx.conf`

```bash
docker run -p 80:80 -v /docker_data/nginx.conf:/etc/nginx/nginx.conf --name blog-admin -d carldu/blog-html-admin:latest
```

## 关于

本项目是作者利用空余时间开发，维护全靠热爱发电。如果使用过程中遇到问题，欢迎报告 issue。
