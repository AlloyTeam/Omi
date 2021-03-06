## 安装  

直接下载并用 `<script>` 标签引入，Omi 会被注册为一个全局变量。

* [Omi 开发版本](https://unpkg.com/omi@latest/dist/omi.js)
* [Omi 压缩版本](https://unpkg.com/omi@latest/dist/omi.min.js)

也可以通过 npm 安装

```bash
npm i omi
```


## 命令行工具

Omi 提供了官方的 CLI，你不需要去学习怎么配置 webpack、babel 或者 TypeScript，CLI 帮你配置好了一切，且提供了各种模板满足不同的项目类型。

```bash
$ npm i omi-cli -g     # install cli
$ omi init my-app      # init project
$ cd my-app            
$ npm start            # develop
$ npm run build        # release
```

> `npx omi-cli init my-app` 也是支持的(npm v5.2.0+).


### npm 脚本

```json
"scripts": {
  "start": "vite",
  "build": "tsc && vite build --base=./",
}
```

你也可以设置 PUBLIC_URL, 比如：

```json
  "build": "tsc && vite build --base=https://your.url.com/sub ",
```

## 项目模板

| **Template Type**|  **Command**|  **Describe**|
| ------------ |  -----------|  ----------------- |
|基础模板(v3.3.0+)|`omi init my-app`| 基础模板|
|Kbone Template|`omi init-kbone my-app`  | 使用 omi 开发小程序或者 Web|
