<h1 align="center">Welcome to hamibot-starter 👋</h1>
<p align="center">
  <a href="https://www.npmjs.com/package/script-template" target="_blank">
    <img alt="Version" src="https://img.shields.io/npm/v/script-template.svg">
  </a>
  <a href="#" target="_blank">
    <img alt="GitHub package.json version" src="https://img.shields.io/github/package-json/v/batu1579/hamibot-starter">
  </a>
  <a href="[#](https://github.com/batu1579/hamibot-starter/blob/main/LICENSE)" target="_blank">
    <img alt="License: MPL--2.0" src="https://img.shields.io/badge/License-MPL--2.0-yellow.svg" />
  </a>
</p>

> 一个用来快速开始编写 `Hamibot` 脚本的模板，使用 `TypeScript` 编写。
>
> 通过声明文件提供 `Hamibot` 绝大部分函数的代码提示、类型检查和文档，帮你减少键入次数和查询官方文档的时间。提供常用的代码片段，直接调用可以辅助更快完成开发，并让你能专注于核心功能。
>
> 欢迎各位大佬帮我一起完善这个项目！

## 安装依赖

> 因为使用了 npm 来管理依赖，在安装之前请确保安装过 `node.js` 。

```sh
npm install
```

## 快速开始

1. 下载本仓库，有两种方式可选：
   1. 点击 [Use this template](https://github.com/batu1579/hamibot-starter/generate) 按钮以此仓库为模板创建一个自己的仓库，然后将仓库克隆到本地。
   2. 如果你不准备使用 Git 作为版本管理工具，可以直接通过 `Code` -> `Download ZIP` 下载压缩包。
2. 在 `.\src` 文件夹下编写代码，程序入口为 `src\index.ts` 。
3. 完成编写后打包项目，有两种方式可选：
   1. 使用 VSCode 快捷键 `ctrl + shift + b` 打开任务菜单，然后选择 `npm build` 打包。
   2. 使用命令打包项目：

      ```sh
      npm run build
      ```

4. 在控制台上传打包后的文件: `.\dist\index.js` 。

## 使用预制函数

所有预制库都存放在 `./src/lib` 文件夹中。

详细使用方式和文档见 [预制库说明](./src/lib/docs/README.md) 。

## 注意事项

1. 编写 UI 或悬浮窗时请记得将文件扩展名修改成 `tsx` 。
2. 如果有用到暂时没有声明过的模块，可以使用 TS 的忽略语法:

   > 注意：忽略会跳过所有检查，除了语法错误。使用时会有风险，请在确保肯定不会出现问题后再使用。

    ```typescript
    // 多行忽略（取消两个标记间的代码检查。）
    // 可以不使用结束标记，即忽略到文件结尾。
    // 注意：必须在文件顶部使用。
    // @ts-nocheck
   
    // 要跳过检查的某段代码
    canvas.drawLine(0, 0, 1080, 1920, paint);
   
    // @ts-check
   
    // 单行忽略（取消下一行的代码检查。）
    // @ts-ignore
    canvas.drawLine(0, 0, 1080, 1920, paint);
    ```

## TODO List

- [ ] 将 hamibot 的类型声明单独发布到 `DefinitelyTyped`
- [ ] 添加声明文件 [24/26]
  - [ ] Util
  - [ ] Canvans
- [ ] 使用 `Eslint` 在提交前统一代码风格
- [ ] 检查泛型注释
- [ ] 检查回调函数注释
- [ ] 检查注释中的类和方法是否使用行内代码格式
- [ ] 检查注释中的示例代码是否都能够运行
- [ ] 统一函数类型（Function、function）

## 作者

👤 **BATU1579**

- Github: [@batu1579](https://github.com/batu1579)

## 支持

如果有帮到你的话，帮我点颗小星星叭~ ⭐️

***
_This README was generated with ❤️ by [readme-md-generator](https://github.com/kefranabg/readme-md-generator)_
