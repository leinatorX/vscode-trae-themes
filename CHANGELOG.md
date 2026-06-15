# Changelog

## 0.1.1 (2026-06-15)

- Deep Blue 主题语法高亮改为 VS2022 Dark+ 经典配色（关键字蓝、类型青绿、函数浅黄、注释绿、字符串橙红、数字浅绿、变量浅蓝、控制流紫、枚举亮蓝）
- Deep Blue 主题通用 `storage` / `storage.type` / `storage.modifier` 改为蓝色 `#569cd6`，修复 `public` / `private` / `class` / `void` 等 C# 关键字在 Roslyn 语义高亮未就绪时仍渲染为紫色的问题
- Deep Blue 主题追加 10 条 `source.cs` 专用规则，覆盖注释 / 关键字 / 控制流 / 修饰符 / 类型 / 方法 / 字段属性 / 字符串（含 verbatim & interpolated）/ 数字 / this-base
- Deep Blue 主题扩展 `semanticTokenColors`，补全 C# Roslyn / C# Dev Kit 语义 token（namespace / class / struct / interface / enum / delegate / type / typeParameter / method / function / property / field / event / variable / parameter / enumMember / constant / keyword / modifier / label / comment / string / number / operator）

## 0.1.0 (2026-05-16)

- 修复终端光标颜色缺失
- 重构主题文件结构：移除 `include` 引用链，扁平化为自包含文件
- 修复 tokenColors 合并问题，补全基础语法高亮规则（注释、字符串、关键字等）
- 补全 `semanticHighlighting: true` 确保语义高亮正确开启
- 删除不再使用的中间引用文件

## 0.0.3 (2026-05-09)

- 修复深蓝主题快捷键提示背景
- 修复深蓝主题编辑区行号增删改标记颜色
- 修复 hex 色值 bug（`ODOEOF` → `0D0E0F`）
- 修复受限模式横幅背景不适配
- 修复行内代码背景色
- 补充 `gitDecoration` 颜色，Git 相关 UI 适配
- 修复焦点边框透明导致部分插件按钮无背景

## 0.0.2 (2026-05-07)

- 修复亮色主题状态栏文字不可见

## 0.0.1 (2026-05-07)

- 初始发布
- 包含 Dark / Deep Blue / Light 三个主题
- 源码来源于 Trae 编辑器
- 修复深蓝主题状态栏透明、边框缺失等 VS Code 不兼容问题
- 修复深蓝主题选项卡、弹窗、终端、输入框等原版遗漏
