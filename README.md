# gallery-by-react
one photo gallery project based on react

#根据慕课网 “React实战-打造画廊应用” 课程完成

 clone 下来直接 npm start 就能运行

或者点击下面在线预览的地址

https://jiujiude.github.io/gallery-by-react/index.html

所用技术栈 React、webpack、sass、ES6，如果npm也算

因为前端工具改版太大，加上React也全面升级为ES6，所以踩过不少坑

个人觉得这个课程挺有代表性，其中有很多东西老师虽然一带而过，但是这要求事后自己再慢慢检查一遍

再查询文档，达到熟悉react工作流程的目的

QQ:393210556

# Start for development
npm start # or
npm run serve

# Start the dev-server with the dist version
npm run serve:dist

# Just build the dist version and copy static files
npm run dist

# Run unit tests
npm test

# Auto-run unit tests on file changes
npm run test:watch

# Lint all files in src (also automatically done AFTER tests are run)
npm run lint

# Clean up the dist directory
npm run clean

# Just copy the static assets
npm run copy


nmp install -g yo  安装http://yeoman.io/
npm install -g generator-react-webpack  安装运行webpack构建react

npm install autoprefixer-loader --save-dev

npm install json-loader --save-dev

npm uninstall node-sass  去官方下载覆盖\node-sass\vendor中的文件进行安装
npm install node-sass@latest


ReactDOM.findDOMNode，当参数是DOM，返回值就是该DOM  等同于 this.refs.xxxxxx 和 this.refs["xxxxxx"]
当参数是Component的时候：获取的是该Component render方法中的DOM
this.refs从组件内部获取组件内部的DOM，ReactDOM.findDOMNode从组件外获取组件渲染的DOM



npm 镜像安装

镜像使用方法（三种办法任意一种都能解决问题，建议使用第三种，将配置写死，下次用的时候配置还在）:
1.通过config命令
npm config set registry https://registry.npm.taobao.org
npm info underscore （如果上面配置正确这个命令会有字符串response）
2.命令行指定

npm --registry https://registry.npm.taobao.org info underscore
3.编辑 ~/.npmrc 加入下面内容
registry = https://registry.npm.taobao.org