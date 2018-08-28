## 反洗钱产品

- 前后端分离，通过token进行数据交互，可独立部署
- 主题定制，通过scss变量统一一站式定制
- 动态菜单，通过菜单管理统一管理访问路由
- 数据切换，通过mock配置对接口数据／mock模拟数据进行切换
- 发布时，可动态配置CDN静态资源／切换新旧版本

## 生成环境，打包并把dist目录文件，部署到Nginx里

构建生产环境(默认) npm run build

```
    # 构建测试环境
    npm run build --qa
    # 构建验收环境
    npm run build --uat
    # 构建生产环境
    npm run build --prod
    # 安装Nginx，并配置Nginx server {
        listen       80;
        server_name  localhost;
    location / {
    root E:\\aml-client; index index.html index.htm;
    } }
    # 启动Nginx后，访问如下路径即可 http://localhost
```