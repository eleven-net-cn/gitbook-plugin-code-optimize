# [gitbook-plugin-code-optimize](https://www.npmjs.com/package/gitbook-plugin-code-optimize)

GitBook 插件，给代码块增加复制按钮，显示行号。fork 自 https://github.com/davidmogar/gitbook-plugin-code ，原始插件不够满足我的开发需求，进行了扩展。

## Installation

直接 install 安装，或者，在 book.json 写入到 plugin 配置后，再运行 gitbook install 命令安装。

NPM

```sh
npm i gitbook-plugin-code-optimize
```

Yarn

```sh
yarn add gitbook-plugin-code-optimize
```

在 book.json 文件增加 plugin、pluginsConfig 配置：

```js
{
  "plugins": ["code-optimize"],
  "pluginsConfig": {
    "code-optimize": {
      "copyButtons": true,
      "showLines": true
    }
  }
}
```

## Constants

| 参数名 | 类型 | 必填 | 默认值 | 说明 |
| ----- | --- | --- | ------ | --- |
| copyButtons | Boolean | 否 | true | 是否开启代码复制 |
| showLines | Boolean | 否 | true | 是否开启显示代码行号 |

## 示例

1. 单行，不显示行号：

    ![single line](https://github.com/davidmogar/gitbook-plugin-code/blob/resources/images/single.png?raw=true)

2. 多行，显示行号：

    ![multi line](https://github.com/davidmogar/gitbook-plugin-code/blob/resources/images/multi.png?raw=true)