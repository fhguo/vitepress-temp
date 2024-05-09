# vitepress-temp

#### 介绍
vitepress-temp是vitepress的项目模板，在原生的基础上使用自定义主题、引入了elementPlus、本地搜索、回到顶部、使用了github actions进行自动化部署静态页面


#### 软件架构

模板基于[VitePress](https://vitepress.dev/zh/)，VitePress 获取用 Markdown 编写的内容，对其应用主题，并生成可以轻松部署到任何地方的静态 HTML 页面。并且项目使用了vue3和[elementPlus](https://element-plus.org/zh-CN/)，可以更好的自定义页面内容。

#### 安装教程

> 提前安装运行环境[nodejs](https://nodejs.org/en)，版本号>=18

1. 安装

   ```bash
   # or pnpm or yarn
   npm install
   ```

2. 运行

   ```bash
   npm run dev
   ```

3. 打包

   ```bash
   npm run docs:build
   ```

#### 使用说明

1.  config文件配置项目，参照[vitepress配置](https://vitepress.dev/zh/reference/site-config)
2.  在theme文件夹自定义主题，参考[自定义主题](https://vitepress.dev/zh/guide/custom-theme)
3.  部署前一定要配置base路径，使用相对路径，相对于服务器根路径的路径
4.  项目部署参考[GitHub Pages](https://vitepress.dev/zh/guide/deploy#github-pages)

#### 参与贡献

1.  Fork 本仓库
2.  新建 Feat_xxx 分支
3.  提交代码
4.  新建 Pull Request
