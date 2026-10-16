# 纸间 · Folio

现代书刊风的 Typora 主题，提供两套配色：

- **Folio / 纸间·昼**：暖白纸色，苔绿点缀。
- **Folio Night / 纸间·夜**：暖炭底色，鼠尾草绿点缀。

正文采用 STIX 英文字体与中文宋体，标题使用黑体；正文宽度随编辑区的 90% 自适应，窄窗口保留少量边距。

## 项目结构

- folio.css：亮色主题入口。
- folio-night.css：暗色主题入口。
- folio/folio-base.css：两套主题共用的排版样式。
- folio/*.woff：随主题附带的 STIX Two Text 字体。
- folio/STIX_2.0.0_license.pdf：字体许可说明。
- folio/样张.md：在 Typora 中检查实际效果的样张。
- folio/preview.html：可切换亮暗配色的浏览器样张。
- folio/README.md：字体配置、样式微调与验证范围。

## 安装与使用

在 Typora 的「偏好设置 → 外观」中打开主题文件夹，将 folio.css、folio-night.css 和整个 folio 文件夹复制进去，保持它们之间的相对位置。

重启 Typora，在「主题」菜单中选择 Folio 或 Folio Night。

## 开发

在项目中修改主题配色或公共排版后，将对应文件复制到 Typora 主题目录，再重新切换主题查看效果。

当前项目是正在使用的纸间主题的完整副本，包含收紧后的标题间距、90% 自适应正文宽度与块元素边缘对齐规则。

## 字体许可

STIX Two Text 的字体许可随字体一并保留，请参阅 folio/STIX_2.0.0_license.pdf。
