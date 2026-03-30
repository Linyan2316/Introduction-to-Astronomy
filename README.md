# Introduction to Astronomy

如果您没有任何天文基础，在阅读《天体物理基础》之前请先阅读《球面天文》第一章和《广义相对论基础》。

此项目还是 demo 版本，尚未注明图片来源，可能有版权风险，请注意。

除却页面和边距、颜色、文献引用设置，其余模版设置放在 Preamble 文件夹中。除去相对路径引用方法，你也可以直接将其放在本地自定义宏包存放文件夹中使用。首先在 terminal 中输入
```shell
kpsewhich -var-value=TEXMFLOCAL
```
确定 texmf-local 文件夹所在路径，然后将模版存放于 texmf-local/tex/latex/local 文件夹中（你可能需要依次建立这一连串文件夹），接着在 terminal 中输入
```shell
texhash
```
更新自定义宏包，最后将 ```.tex``` 文件中的 ```\usepackage{../../Preamble/LinyanPreamble}``` 修改为 ```\usepackage{LinyanPreamble}``` 即可成功使用。此外，你可能需要根据模版设置安装必要的字体。
```shell
brew install font-lxgw-wenkai
brew install font-maple-mono-cn
brew install font-latin-modern-math
```