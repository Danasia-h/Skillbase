---
name: generate-ai-icon
description: Generates playful and boutique-style SVG functional icons for AI assistant systems (menu, send, user, settings, etc.). Directly writes SVG XML code. Use when the user asks to create system icons, UI icons, functional icons, or interface elements for AI assistant applications.
---

# Generate AI System Icons

生成 Playful/Boutique 风格的功能图标（menu, send, user, settings 等）。

## Quick Start

1. 编写 SVG XML 代码（主色 `#4A5568`，stroke-width `2.5`）
2. 使用 Write 工具保存至本 skill 的 `resources/<功能名称>.svg`
3. 输出为标准 24x24 矢量图，可直接用于 HTML/React/img 引用

## 辅助文档

| 文档 | 何时读取 | 内容 |
|------|---------|------|
| **ANIMATION-DECISION-GUIDE.md** | 不确定是否该添加动画 | 详细决策规则、案例分析、性能优化 |
| **SVG-QUICK-REFERENCE.md** | 需要代码模板、忘记语法 | 元素速查、动画模板、常见错误 |
| **ICON-EXAMPLES.md** | 需要完整图标代码 | 50个完整 SVG 图标代码示例 |

## 核心方法

**直接编写 SVG XML 代码**，使用 Write 工具保存（不使用 GenerateImage）。

```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <line x1="4" y1="6" x2="20" y2="6" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

## 工作流程

### 1. 判断生成范围

- **全面生成**："生成图标" → 生成 10-15 个核心图标
- **针对性生成**："生成用户相关图标" → 只生成该模块

### 2. 判断是否需要动画

**必须动画**（表示进行中状态）：
- loading, syncing, processing, refresh

**建议动画**（吸引注意）：
- notification（波浪扩散）, alert（脉动）, like（心跳）

**默认静态**（常规功能）：
- menu, search, user, edit, delete 等

**详细规则** → 读取 [ANIMATION-DECISION-GUIDE.md](ANIMATION-DECISION-GUIDE.md)

### 3. 检查现有图标

- **空文件夹** → 选择配色方案（主色 `#4A5568` + 点缀色）
- **有图标** → 读取 2-3 个，提取 stroke-width、颜色、圆角参数，严格保持一致

### 4. 编写 SVG 代码

**标准模板**：
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <!-- 图标元素 -->
  <line ... stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <circle ... fill="#FF9D9A"/>
</svg>
```

**快速参考** → 读取 [SVG-QUICK-REFERENCE.md](SVG-QUICK-REFERENCE.md)

### 5. 使用 Write 工具保存

**路径约定**（本 skill 目录下的 `resources/`）：

| 场景 | 路径 | 示例 |
|------|------|------|
| 单个/少量图标 | `.cursor/skills/generate-ai-icon/resources/<功能名称>.svg` | `.../resources/menu.svg` |
| 批量生成（按日期归档） | `.cursor/skills/generate-ai-icon/resources/<YYYY-MM-DD>/<功能名称>.svg` | `.../resources/2026-02-11/menu.svg` |

- 若 `resources/` 不存在，先创建目录
- 与 [ICON-EXAMPLES.md](ICON-EXAMPLES.md) 中示例路径保持一致

### 6. 可选：Figma 集成

如用户提供 Figma URL：
1. 使用 Figma MCP 的「获取文件数据」工具（如 `get_figma_data`）
2. 使用 Figma MCP 的「下载图片」工具（如 `download_figma_images`）
3. 分析风格，生成缺失图标

> **说明**：MCP 工具名可能随环境变化（如 `mcp_Framelink_Figma_MCP_*` 或 `user-Framelink_Figma_MCP_*`），以 Agent 当前可用工具为准。

**详细步骤** → 见文档末尾 "Figma 集成指南"

---

## 设计原则

### Playful & Boutique 风格

- ✅ 圆润笔触（stroke-width: 2.5）、圆润端点（stroke-linecap: round）
- ✅ 精品配色（柔和炭灰 `#4A5568` + 点缀色：珊瑚粉 `#FF9D9A`、薄荷绿 `#9FEDD7`）
- ✅ 所有尖角圆角化（rx="4" 或更大）
- ✅ 简洁（每个图标 3-5 个元素，10-15 行代码）
- ❌ 避免：纯黑 `#000000`、细线条、尖锐棱角、复杂细节

### 配色方案

| 颜色 | Hex | 用途 |
|------|-----|------|
| 柔和炭灰 | `#4A5568` | 主线条（必需） |
| 珊瑚粉 | `#FF9D9A` | 点缀、装饰 |
| 薄荷绿 | `#9FEDD7` | 背景填充 |
| 淡紫 | `#C2A8E0` | 次要装饰 |
| 柠檬黄 | `#F4D06F` | 警告高亮 |

---

## SVG 代码示例

### 基础图标

**menu.svg** - 三条线
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <line x1="4" y1="6" x2="20" y2="6" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <line x1="4" y1="12" x2="20" y2="12" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <line x1="4" y1="18" x2="20" y2="18" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

**user.svg** - 头像
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <circle cx="12" cy="8" r="4" stroke="#4A5568" stroke-width="2.5"/>
  <path d="M 4 20 C 4 16 7.5 14 12 14 C 16.5 14 20 16 20 20" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

**search.svg** - 放大镜
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <circle cx="10" cy="10" r="6" stroke="#4A5568" stroke-width="2.5"/>
  <line x1="15" y1="15" x2="20" y2="20" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

**更多示例** → 读取 [ICON-EXAMPLES.md](ICON-EXAMPLES.md)（50个完整图标代码）

### 动画图标

**loading-animated.svg** - 旋转
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <style>
    @keyframes rotate { from { transform: rotate(0deg); } to { transform: rotate(360deg); } }
    .spinner { animation: rotate 1.5s linear infinite; transform-origin: center; }
  </style>
  <g class="spinner">
    <path d="M 12 3 A 9 9 0 0 1 21 12" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" fill="none"/>
    <circle cx="12" cy="3" r="2" fill="#FF9D9A"/>
  </g>
</svg>
```

**notification-wave.svg** - 波浪扩散
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <style>
    @keyframes wave { 0% { transform: scale(0.8); opacity: 1; } 100% { transform: scale(1.5); opacity: 0; } }
    .wave1 { animation: wave 2s ease-out infinite; }
    .wave2 { animation: wave 2s ease-out 0.5s infinite; }
  </style>
  <!-- 铃铛 -->
  <path d="M 8 8 C 8 5.8 9.8 4 12 4 C 14.2 4 16 5.8 16 8 L 16 14 L 8 14" stroke="#4A5568" stroke-width="2.5"/>
  <!-- 通知点 + 波浪 -->
  <circle cx="18" cy="6" r="3" fill="#FF9D9A"/>
  <circle cx="18" cy="6" r="3" stroke="#FF9D9A" stroke-width="1.5" fill="none" class="wave1"/>
  <circle cx="18" cy="6" r="3" stroke="#FF9D9A" stroke-width="1.5" fill="none" class="wave2"/>
</svg>
```

**更多动画示例** → 读取 [ANIMATION-DECISION-GUIDE.md](ANIMATION-DECISION-GUIDE.md)

---

## 完整图标清单

### 核心（14个，优先生成）
- menu, home, back, forward, close, more
- send, message, notification
- user, settings, search
- edit, delete

### 操作类（8个）
- add, save, copy, paste, undo, redo, refresh, download

### 系统类（6个）
- filter, help, info, warning, security, theme

### 文件类（6个）
- file, folder, upload, attach, image, document

### 状态类（6个）
- success, error, loading, favorite, like, bookmark

### 用户账户类（4个）
- users, login, logout, profile

### 媒体类（5个，可选）
- play, pause, stop, volume, mute

**总计**：约 50 个

---

## SVG 技术规范

### 必需属性

```xml
xmlns="http://www.w3.org/2000/svg"
width="24" height="24"
viewBox="0 0 24 24"
stroke-width="2.5"
stroke-linecap="round"
stroke-linejoin="round"
```

### 常用元素

- `<line>` - 直线
- `<circle>` - 圆形  
- `<rect rx="4">` - 圆角矩形
- `<path d="M... L...">` - 复杂路径

### 路径命令

| 命令 | 说明 |
|------|------|
| `M x y` | 移动到 |
| `L x y` | 直线到 |
| `C x1 y1 x2 y2 x y` | 贝塞尔曲线 |
| `A rx ry 0 0 1 x y` | 圆弧 |
| `Z` | 闭合 |

---

## 质量检查

- [ ] 功能清晰、易识别
- [ ] 使用精品配色（非纯黑）
- [ ] stroke-width 一致
- [ ] 所有尖角已圆角化
- [ ] 文件 < 5KB（纯文本 XML）
- [ ] 用文本编辑器可打开
- [ ] 如有动画，已添加 `prefers-reduced-motion` 支持

---

## 常见问题

**Q: 如何确保风格一致？**  
A: 读取现有图标，提取 stroke-width、颜色等参数，严格使用相同值。

**Q: 何时添加动画？**  
A: 默认静态。loading/notification 等必须或建议添加动画。详见 [ANIMATION-DECISION-GUIDE.md](ANIMATION-DECISION-GUIDE.md)

**Q: 如何验证是真 SVG？**  
A: 文本编辑器打开应看到 `<svg>` 标签，文件 < 5KB。

**Q: 可以从 Figma 导入吗？**  
A: 可以！使用 Figma MCP 工具。详见下方"Figma 集成指南"。

---

## 输出使用与协同

### 直接使用

生成的 SVG 保存在 **本 skill 的 `resources/`**，为标准矢量图，可：

- **HTML**：复制到项目后 `<img src="assets/menu.svg" />`
- **React**：复制到项目后导入，或内联 SVG 代码
- **内联**：复制 SVG 代码直接嵌入 JSX/HTML

### 与其他 Skill 协同

| 协同对象 | 用法 |
|----------|------|
| **create-rule** | 规则中可约定从 `.cursor/skills/generate-ai-icon/resources/` 引用图标 |
| **Figma MCP** | 从 Figma 获取设计稿后，按本 skill 规范生成风格一致的缺失图标至 skill resources |
| **前端项目** | 将 skill 中 `resources/` 的图标复制到项目 `public/assets/` 等目录后引用 |

---

## Figma 集成指南

### 快速流程

1. **获取数据**：调用 Figma MCP 的 get_figma_data（fileKey, nodeId）
2. **下载图标**：调用 Figma MCP 的 download_figma_images（localPath 用绝对路径）
3. **分析风格**：读取下载的 SVG，提取 stroke-width、颜色
4. **生成缺失**：编写新图标，匹配 Figma 参数

### Figma URL 格式

```
https://www.figma.com/file/<fileKey>/<fileName>
https://www.figma.com/design/<fileKey>/<fileName>?node-id=<nodeId>
```

### MCP 工具调用示例

> 工具名以 Agent 当前环境为准（可能为 `mcp_Framelink_Figma_MCP_*` 等前缀）。

**获取数据**（get_figma_data）：
```javascript
{ fileKey: "abc123", nodeId: "10:50" }  // nodeId 可选
```

**下载图标**（download_figma_images）：
```javascript
{
  fileKey: "abc123",
  localPath: "<workspace>/.cursor/skills/generate-ai-icon/resources",  // 本 skill 的 resources 绝对路径，用正斜杠
  nodes: [
    { nodeId: "10:51", fileName: "menu.svg" },
    { nodeId: "10:52", fileName: "send.svg" }
  ]
}
```

### Figma 最佳实践

1. **命名规范**：Figma 中命名为 `icon/menu` → 下载为 `menu.svg`
2. **使用 Component**：便于 Agent 识别
3. **统一 Styles**：在 Figma 中设置统一的 strokeWeight、cornerRadius
4. **24x24px**：确保图标尺寸标准化

### 故障排除

- **路径错误**：使用绝对路径，Windows 用 `/` 不用 `\`
- **找不到节点**：确保是 Component 类型
- **风格不一致**：检查 Figma 是否使用统一 Styles

---

## 辅助文档

本 skill 包含详细参考文档，在需要时读取：

| 文档 | 何时读取 |
|------|---------|
| **ANIMATION-DECISION-GUIDE.md** | 不确定是否该添加动画、需要案例分析 |
| **SVG-QUICK-REFERENCE.md** | 需要代码模板、忘记语法、快速查找示例 |
| **ICON-EXAMPLES.md** | 需要查看 50 个完整图标的代码示例 |
