# 项目目录规范

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

每个项目都必须「MUST」包含一个`README.md`文件，此文件中应当「SHOULD」概要描述此项目的功能和特点等信息。

### .editorconfig

每个项目应当「SHOULD」包含`.editorconfig`，用来统一配置编辑器的换行、缩进存储格式，使用方式请参考[editorconfig是什么？](https://github.com/fex-team/styleguide/blob/master/editorconfig.md)。

### src

项目中所有 JS 源码应当「SHOULD」存放在此目录下，且所有JS文件编写应当「SHOULD」遵循[Javascript 编码规范](https://github.com/fex-team/styleguide/blob/master/javascript.md)。

### css、themes、less、sass

样式类文件存放应当「SHOULD」遵循以下规律，且文件编写应当「SHOULD」遵循[CSS 编码规范](https://github.com/fex-team/styleguide/blob/master/css.md)。

* 不带主题的样式文件应当「SHOULD」统一存放在 css 目录下面，且样式中使用的背景图片资源应当「SHOULD」统一存放在 `css/images` 目录下面。
* 带主题的样式文件应当「SHOULD」统一存放在 themes 目录下对应的主题目录下，默认的主题应当「SHOULD」采用 `default` 作为主题名称，且应当「SHOULD」默认提供，样式中对应图片文件应当「SHOULD」存放在样式文件所在的主题目录下的 `images` 目录下。
* less 格式的样式文件应当「SHOULD」统一存放在 `less` 目录下面。
* sass 格式的样式文件应当「SHOULD」统一存放在 `sass` 目录下面。

### examples

存放详细的示例文件

### doc

所有项目应当「SHOULD」包含一个 `doc` 目录，用来存放详细的 API 使用文档。

### dist

dist 作为项目输出目录，所有编译生成、提供给用户使用的文件应当「SHOULD」存放在此目录。

为了让不太擅长 node.js 的用户可以正常使用编译后的代码，dist 目录应当「SHOULD」包含基本输出结果并提交在 github 中。

### build

所有工具类脚本应当「SHOULD」放在此目录。

### test

所有测试相关代码应当「SHOULD」放在此目录。
