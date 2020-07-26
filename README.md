## 开发

```bash
# 克隆项目
git clone https://gitee.com/y_project/RuoYi-Vue

# 进入项目目录
cd ruoyi-ui

# 安装依赖
npm install

# 建议不要直接使用 cnpm 安装依赖，会有各种诡异的 bug。可以通过如下操作解决 npm 下载速度慢的问题
npm install --registry=https://registry.npm.taobao.org

# 启动服务
npm run dev
```

浏览器访问 http://localhost:80

## 发布

```bash
# 构建测试环境
npm run build:stage

# 构建生产环境
npm run build:prod
```

## 依赖说明

```bash
clipboard：
file-saver：
js-beautify：美化代码，代码生成时用到
fuse.js：模糊查询，顶部搜索区域用到
js-cookie：操作cookie，登录注销用到
jsencrypt：加密数据，加密密码时用到
normalize.css：解决各浏览器样式的不一致性
nprogress：路由跳转时顶部显示的进度条
```