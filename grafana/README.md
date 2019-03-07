# grafana汉化
汉化分为前端部分和后端部分，前端需要Node.js环境，后端需要golang环境，在调试开发过程中需要修改conf/defaults.ini中值
app_mode = development

## 前端汉化
大部分内容在前端汉化，主要是public文件夹下<br />
编译前端命令：<br />
1、下载依赖：npm install <br />
2、运行查看：npm start <br />
3、打包前端：npm run-script build <br />


## 后端汉化
后端汉化部分比较少，主要是左侧菜单的汉化是在后端存储的。
主要汉化pkg/api/index.go文件中，修改完成后输入命令：<br/>
构建下载依赖：go run build.go setup <br />
构建后端打包命令：go run build.go build <br />
执行完命令后在bin文件中能看到刚刚编译的可执行文件 <br />

