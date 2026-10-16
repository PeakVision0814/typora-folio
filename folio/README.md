# 纸间 · Folio

现代书刊风的 Typora 主题，提供暖白苔绿的 Folio 与暖炭鼠尾草绿的 Folio Night。

## 启用

主题已放入 Typora 的 themes 目录。重启 Typora，然后在「主题」菜单选择 **Folio** 或 **Folio Night**。

在本地打开 `preview.html` 可切换两套配色，检查中英文、表格、代码和脚注的样式。此页是浏览器对照预览，不包含真实的 Typora 编辑器交互。

## 字体与排版

- 中文正文优先使用思源宋体 / Noto Serif SC，未安装时回退到系统宋体。
- 英文正文使用随主题附带的 STIX Two Text；中文标题与界面优先使用 Noto Sans SC，再回退到微软雅黑等系统字体。
- 代码使用本机 Cascadia Code、JetBrains Mono 或 Consolas，无需在线加载字体。
- 公式保留 Typora 自带的数学字体，不修改 MathJax 字形度量。
- 正文 17px、1.8 倍行高，正文宽度为编辑区的 90%，随窗口自适应；窄屏使用全宽并保留少量内边距。
- PDF / 打印使用白底深色文字；HTML 导出保留当前主题配色。

## 微调

两种配色分别在 `../folio.css`、`../folio-night.css`，共同排版在 `folio-base.css`。

例如修改公共文件中的以下变量：

```css
:root {
    --folio-body-size: 17px;
    --folio-line-height: 1.8;
    --folio-reading-width: 90%; /* 相对编辑区的正文宽度 */
}
```

复制主题到其他电脑时，请同时复制 `folio.css`、`folio-night.css` 和整个 `folio` 文件夹。

## 字体许可

STIX 字体从原 Academic 主题附带的本地文件复制，许可见 `STIX_2.0.0_license.pdf`。

## 验证范围

浏览器样张用于检查配色、字体、窄屏布局和打印 CSS。Typora 的实时编辑、源代码模式、行号、公式与导出应使用自己的 Markdown 文档在实际应用中检查。

已用本机 Edge 无头渲染检查亮暗样张：1440、700、420、360px 下均无页面横向溢出，字体资源正常加载；两种主题的打印 CSS 均为白底深色文字。正文、链接、引用、侧栏文字与代码语法颜色均按至少 4.5:1 的文字对比度检查。此记录不代表真实 Typora 编辑与导出已实测。
