### 构建ts webpack项目
```
npm init -y
cnpm install typescript -g
tsc --init    生成tsconfig.json 文件
npm install typescript

cnpm install tslint -g
tslint -i

npm install webpack webpack-cli webpack-dev-server -D
npm install html-webpack-plugin clean-webpack-plugin -D
npm install ts-loader -D

npm install cross-env
```

##### package.json
```
"scripts": {
    "start": "cross-env NODE_ENV=development webpack-dev-server --mode=development --config webpack.config.js",
    "build": "cross-env NODE_ENV=production webpack --mode=production --config webpack.config.js"
  },
```

