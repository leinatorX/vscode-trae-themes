# Changelog

## 0.2.0 (2026-06-15)

- 三个主题（Deep Blue / Dark / Light）代码配色统一改为 VS2022 经典风格：
  - 暗色系（Deep Blue、Dark）：关键字 `#569cd6`、类型 `#4ec9b0`、函数 `#dcdcaa`、注释 `#6A9955`、字符串 `#ce9178`、数字 `#b5cea8`、变量 `#9cdcfe`、控制流 `#c586c0`、枚举 `#4fc1ff`、标签 `#c8c8c8`
  - 浅色（Light）：关键字 `#0000ff`、类型 `#267f99`、函数 `#795e26`、注释 `#008000`、字符串 `#a31515`、数字 `#098658`、变量 `#001080`、控制流 `#af00db`、枚举 `#0070c1`、标签 `#000000`
- 三主题通用 `storage` / `storage.type` / `storage.modifier` 一并改为关键字色，修复 C# `public` / `private` / `class` / `void` 等在 Roslyn 语义高亮未就绪时回退为紫色的闪烁问题
- 三主题各追加 10 条 `source.cs` 专用规则（注释 / 关键字 / 控制流 / 修饰符 / 类型 / 方法 / 字段属性 / 字符串含 verbatim & interpolated / 数字 / this-base）
- 三主题 `semanticTokenColors` 从 4 条扩展到 28 条，补全 C# Roslyn / C# Dev Kit 语义 token
- Deep Blue 主题 `editor.lineHighlightBackground` 由 `#282B3A` 改为 `#0000003F`（半透明黑色叠加），减弱当前行高亮阴影对比度
- Deep Blue 主题 `tab.activeBorderTop` 由 `#FFFFFF` 改为 `#00BCD480`（青绿半透明），活跃标签顶部白线改为柔和的青色高亮
- README 新增 Unity / C# 推荐 settings 片段

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
