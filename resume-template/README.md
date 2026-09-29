# 简历模板（LaTeX · 一页 A4 · 中文）

脱敏的保研 / 求职简历模板，基于 XeLaTeX + ctexart，编译产物恰好一页 A4。

## 使用方法

1. 用编辑器打开 `resume-template.tex`，把所有 `XX` / 占位符替换成你自己的信息。
2. 证件照命名为 `photo.jpg` 放在本目录（没有照片也能编译，会显示占位框）。
3. 编译（需安装 TeX 发行版，如 TeX Live / MiKTeX）：

   ```bash
   xelatex resume-template.tex
   ```

   跑一次即可（本模板无页眉页脚 overlay，不需要跑两次）。

## 字体说明

- 默认中文微软雅黑（`Microsoft YaHei`）、英文 Times New Roman，Windows 自带。
- macOS：把 `Microsoft YaHei` 换成 `PingFang SC`；Linux：换成 `Noto Sans CJK SC`。

## 定制

- **主题色**：`\definecolor{theme}{RGB}{126, 12, 110}` 改成目标院校主色（如北大红 `176,7,30`、清华紫 `102,8,116`）。
- **加校徽页眉页脚**：如需校徽，可用 `tikz` 的 `remember picture, overlay` 定位（见原版思路），本模板为通用起见已移除。
