# SVG 快速参考

生成 SVG 矢量图的代码速查表。

## 基本模板

```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <!-- 图标元素 -->
</svg>
```

## 必需属性

| 属性 | 值 | 说明 |
|------|-----|------|
| `xmlns` | `"http://www.w3.org/2000/svg"` | 必需 |
| `width` / `height` | `"24"` | 尺寸 |
| `viewBox` | `"0 0 24 24"` | 坐标系 |
| `stroke-width` | `"2.5"` | 整套统一 |
| `stroke-linecap` | `"round"` | 圆润端点 |
| `stroke-linejoin` | `"round"` | 圆润连接 |

## 常用元素

**直线**
```xml
<line x1="4" y1="12" x2="20" y2="12" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
```

**圆形**
```xml
<circle cx="12" cy="12" r="8" stroke="#4A5568" stroke-width="2.5" fill="none"/>
```

**矩形（圆角）**
```xml
<rect x="4" y="4" width="16" height="16" rx="4" stroke="#4A5568" stroke-width="2.5" fill="none"/>
```

**路径**
```xml
<path d="M 4 12 L 20 12" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" fill="none"/>
```

**折线**
```xml
<polyline points="4,12 12,4 20,12" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" fill="none"/>
```

## 路径命令

| 命令 | 说明 | 示例 |
|------|------|------|
| `M x y` | 移动到 | `M 4 12` |
| `L x y` | 直线到 | `L 20 12` |
| `H x` / `V y` | 水平/垂直线 | `H 20` / `V 20` |
| `C x1 y1 x2 y2 x y` | 贝塞尔曲线 | `C 4 8 8 4 12 4` |
| `A rx ry 0 0 1 x y` | 圆弧 | `A 8 8 0 0 1 20 12` |
| `Z` | 闭合路径 | `Z` |

## 配色方案

| 颜色 | Hex | 用途 |
|------|-----|------|
| 柔和炭灰 | `#4A5568` | 主线条（必需） |
| 珊瑚粉 | `#FF9D9A` | 点缀 |
| 薄荷绿 | `#9FEDD7` | 填充 |
| 淡紫 | `#C2A8E0` | 装饰 |
| 柠檬黄 | `#F4D06F` | 高亮 |

## 动画模板

### 旋转（loading, refresh）

```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <style>
    @keyframes rotate { from { transform: rotate(0deg); } to { transform: rotate(360deg); } }
    .spinner { animation: rotate 1.5s linear infinite; transform-origin: center; }
  </style>
  <g class="spinner">
    <path d="M 12 3 A 9 9 0 0 1 21 12" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" fill="none"/>
  </g>
</svg>
```

### 脉动（notification, alert）

```xml
<style>
  @keyframes pulse { 0%, 100% { transform: scale(1); } 50% { transform: scale(1.2); opacity: 0.7; } }
  .pulse { animation: pulse 2s ease-in-out infinite; transform-origin: center; }
</style>
<circle class="pulse" cx="18" cy="6" r="3" fill="#FF9D9A"/>
```

### 波浪扩散（notification, broadcast）

```xml
<style>
  @keyframes wave { 0% { transform: scale(0.8); opacity: 1; } 100% { transform: scale(1.5); opacity: 0; } }
  .wave1 { animation: wave 2s ease-out infinite; }
  .wave2 { animation: wave 2s ease-out 0.5s infinite; }
</style>
<circle class="wave1" cx="18" cy="6" r="3" stroke="#FF9D9A" fill="none"/>
<circle class="wave2" cx="18" cy="6" r="3" stroke="#FF9D9A" fill="none"/>
```

### 心跳（like, favorite）

```xml
<style>
  @keyframes heartbeat { 0%, 100% { scale(1); } 10% { scale(1.2); } 20% { scale(1); } 30% { scale(1.15); } }
  .heart { animation: heartbeat 2s ease-in-out infinite; transform-origin: center; }
</style>
<g class="heart">
  <path d="M 12 21 C 12 21 3 14 3 9 C 3 6 5 4 7 4 C 9 4 11 5 12 7 C 13 5 15 4 17 4 C 19 4 21 6 21 9 C 21 14 12 21 12 21 Z" stroke="#4A5568" stroke-width="2.5" fill="#FF9D9A" fill-opacity="0.3"/>
</g>
```

### 动画参数

| 类型 | 周期 | 缓动 | 场景 |
|------|------|------|------|
| rotate | 1-2s | linear | loading, sync |
| pulse | 2-3s | ease-in-out | notification, alert |
| wave | 2-3s | ease-out | broadcast |
| heartbeat | 2s | ease-in-out | like, favorite |

### 可访问性

```css
@media (prefers-reduced-motion: reduce) {
  .spinner, .pulse, .wave1, .wave2, .heart {
    animation: none !important;
  }
}
```

## 常见错误

| 错误 | 正确 |
|------|------|
| ❌ 使用 GenerateImage 工具 | ✅ 直接编写 XML 代码 |
| ❌ 忘记 `xmlns` | ✅ 必需包含 |
| ❌ 纯黑 `#000000` | ✅ 使用 `#4A5568` |
| ❌ 细线条 `stroke-width="1"` | ✅ 使用 `"2.5"` |
| ❌ 忘记 `stroke-linecap="round"` | ✅ 所有线条都加 |

## 完整示例

**更多示例** → 读取 [ICON-EXAMPLES.md](ICON-EXAMPLES.md)（50个完整图标）
