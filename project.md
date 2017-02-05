# 开源项目目录规范

## 项目命名

全部采用小写方式， 以下划线分隔。

例：`my_project_name`

## 目录命名

参照项目命名规则；

有复数结构时，要采用复数命名法。

例：`scripts`, `styles`, `images`, `data_models`

## CSS、JS文件命名

参照项目命名规则。

例：`account_model.js`


## 目录规范

参加的目录结构为：

```
.
├── .editorconfig
├── css
├── dist
├── examples
├── README.md
├── src
```

### README.md

每个项目都必须「MUST」包含一个`README.md`文件，此文件中应当概要描述此项目的功能和特点等信息。

### .editorconfig

每个项目应当包含`.editorconfig`，用来统一配置编辑器的换行、缩进存储格式。
### src

项目中所有 JS 源码应当存放在此目录下

### css、themes、less、sass

项目中所有样式类文件应当存放在此目录下

### examples

存放详细的示例文件

### doc

所有项目应当包含一个 `doc` 目录，用来存放详细的 API 使用文档。

### dist

dist 作为项目输出目录，所有编译生成、提供给用户使用的文件应当存放在此目录。

为了让不太擅长 node.js 的用户可以正常使用编译后的代码，dist 目录应当包含基本输出结果并提交在 github 中。

### build

所有工具类脚本应当放在此目录。

### test

所有测试相关代码应当放在此目录。
