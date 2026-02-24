# 图标代码示例库

50 个完整的 SVG 图标代码，按功能分类。

## 使用说明

- 直接复制代码，使用 Write 工具保存
- 所有图标使用相同参数：stroke-width="2.5", stroke="#4A5568"
- 点缀色：珊瑚粉 `#FF9D9A`、薄荷绿 `#9FEDD7`

---

## 核心导航类

### menu.svg - 菜单
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <line x1="4" y1="6" x2="20" y2="6" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <line x1="4" y1="12" x2="20" y2="12" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <line x1="4" y1="18" x2="20" y2="18" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

### home.svg - 首页
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 3 12 L 12 3 L 21 12" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M 5 10 L 5 20 C 5 21 6 22 7 22 L 17 22 C 18 22 19 21 19 20 L 19 10" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### back.svg - 返回
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <line x1="19" y1="12" x2="5" y2="12" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <polyline points="12,5 5,12 12,19" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" fill="none"/>
</svg>
```

### forward.svg - 前进
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <line x1="5" y1="12" x2="19" y2="12" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <polyline points="12,5 19,12 12,19" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" fill="none"/>
</svg>
```

### close.svg - 关闭
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <line x1="6" y1="6" x2="18" y2="18" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <line x1="18" y1="6" x2="6" y2="18" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

### more.svg - 更多
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <circle cx="12" cy="6" r="2" fill="#4A5568"/>
  <circle cx="12" cy="12" r="2" fill="#4A5568"/>
  <circle cx="12" cy="18" r="2" fill="#4A5568"/>
</svg>
```

---

## 消息/通信类

### send.svg - 发送
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 3 3 L 21 12 L 3 21 L 7 12 Z" stroke="#4A5568" stroke-width="2.5" stroke-linejoin="round" fill="none"/>
  <line x1="7" y1="12" x2="21" y2="12" stroke="#4A5568" stroke-width="2.5"/>
  <circle cx="18" cy="6" r="2" fill="#FF9D9A"/>
</svg>
```

### message.svg - 消息
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <rect x="3" y="5" width="18" height="14" rx="4" stroke="#4A5568" stroke-width="2.5"/>
  <path d="M 3 8 L 12 13 L 21 8" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### notification.svg - 通知（静态）
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 8 8 C 8 5.8 9.8 4 12 4 C 14.2 4 16 5.8 16 8 L 16 14 C 16 14 17 15 18 16 L 6 16 C 7 15 8 14 8 14 Z" stroke="#4A5568" stroke-width="2.5" stroke-linejoin="round" fill="none"/>
  <line x1="12" y1="4" x2="12" y2="2" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <path d="M 10 18 C 10 19 11 20 12 20 C 13 20 14 19 14 18" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <circle cx="18" cy="6" r="3" fill="#FF9D9A"/>
</svg>
```

### comment.svg - 评论
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <rect x="3" y="4" width="18" height="14" rx="4" stroke="#4A5568" stroke-width="2.5"/>
  <path d="M 9 18 L 12 21 L 12 18" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### reply.svg - 回复
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 9 12 L 4 7 L 9 2" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" fill="none"/>
  <path d="M 4 7 L 14 7 C 18 7 20 9 20 13 L 20 22" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### voice.svg - 语音
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <rect x="9" y="3" width="6" height="11" rx="3" stroke="#4A5568" stroke-width="2.5"/>
  <path d="M 5 10 L 5 12 C 5 16 8 19 12 19 C 16 19 19 16 19 12 L 19 10" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <line x1="12" y1="19" x2="12" y2="22" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

### call.svg - 电话
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 22 17 L 22 20 C 22 21 21 22 20 22 C 9 22 2 15 2 4 C 2 3 3 2 4 2 L 7 2 C 8 2 9 3 9 4 L 9 8 L 6 10 C 7 13 11 17 14 18 L 16 15 L 20 15 C 21 15 22 16 22 17 Z" stroke="#4A5568" stroke-width="2.5" stroke-linejoin="round" fill="none"/>
</svg>
```

### video.svg - 视频通话
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <rect x="2" y="6" width="14" height="12" rx="3" stroke="#4A5568" stroke-width="2.5"/>
  <path d="M 16 10 L 22 6 L 22 18 L 16 14" stroke="#4A5568" stroke-width="2.5" stroke-linejoin="round" fill="none"/>
</svg>
```

---

## 用户/账户类

### user.svg - 用户
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <circle cx="12" cy="8" r="4" stroke="#4A5568" stroke-width="2.5"/>
  <path d="M 4 20 C 4 16 7.5 14 12 14 C 16.5 14 20 16 20 20" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

### users.svg - 多用户
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <circle cx="9" cy="7" r="3" stroke="#4A5568" stroke-width="2.5"/>
  <circle cx="16" cy="7" r="3" stroke="#C2A8E0" stroke-width="2.5"/>
  <path d="M 2 18 C 2 15 5 13 9 13 C 10.5 13 12 13.5 12 13.5" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <path d="M 12.5 18 C 12.5 15 15 13 18 13 C 21 13 23 15 23 18" stroke="#C2A8E0" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

### login.svg - 登录
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 15 3 L 19 3 C 20 3 21 4 21 5 L 21 19 C 21 20 20 21 19 21 L 15 21" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <polyline points="10,7 15,12 10,17" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" fill="none"/>
  <line x1="3" y1="12" x2="15" y2="12" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

### logout.svg - 登出
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 9 3 L 5 3 C 4 3 3 4 3 5 L 3 19 C 3 20 4 21 5 21 L 9 21" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <polyline points="14,7 9,12 14,17" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" fill="none"/>
  <line x1="21" y1="12" x2="9" y2="12" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

### profile.svg - 个人中心
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <circle cx="12" cy="12" r="9" stroke="#4A5568" stroke-width="2.5"/>
  <circle cx="12" cy="10" r="3" stroke="#4A5568" stroke-width="2.5"/>
  <path d="M 6 19 C 6 16 8.5 14 12 14 C 15.5 14 18 16 18 19" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

---

## 操作/编辑类

### edit.svg - 编辑
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 17 3 L 21 7 L 9 19 L 3 21 L 5 15 Z" stroke="#4A5568" stroke-width="2.5" stroke-linejoin="round" fill="none"/>
  <path d="M 17 3 L 21 7 L 19 9 L 15 5 Z" fill="#FF9D9A"/>
  <line x1="15" y1="5" x2="19" y2="9" stroke="#4A5568" stroke-width="2.5"/>
</svg>
```

### delete.svg - 删除
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <line x1="5" y1="7" x2="19" y2="7" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <path d="M 9 7 V 5 C 9 4 10 3 11 3 L 13 3 C 14 3 15 4 15 5 V 7" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <path d="M 6 7 L 7 20 C 7 21 8 22 9 22 L 15 22 C 16 22 17 21 17 20 L 18 7" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="10" y1="11" x2="10" y2="18" stroke="#4A5568" stroke-width="2" stroke-linecap="round"/>
  <line x1="14" y1="11" x2="14" y2="18" stroke="#4A5568" stroke-width="2" stroke-linecap="round"/>
</svg>
```

### add.svg - 添加
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <circle cx="12" cy="12" r="10" stroke="#4A5568" stroke-width="2.5"/>
  <line x1="12" y1="7" x2="12" y2="17" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <line x1="7" y1="12" x2="17" y2="12" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

### save.svg - 保存
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 19 21 L 5 21 C 4 21 3 20 3 19 L 3 5 C 3 4 4 3 5 3 L 16 3 L 21 8 L 21 19 C 21 20 20 21 19 21 Z" stroke="#4A5568" stroke-width="2.5" stroke-linejoin="round"/>
  <rect x="7" y="3" width="6" height="6" rx="1" fill="#9FEDD7"/>
  <line x1="8" y1="15" x2="16" y2="15" stroke="#4A5568" stroke-width="2" stroke-linecap="round"/>
</svg>
```

### copy.svg - 复制
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <rect x="9" y="9" width="13" height="13" rx="3" stroke="#4A5568" stroke-width="2.5"/>
  <path d="M 5 15 L 2 15 L 2 2 L 15 2 L 15 5" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### paste.svg - 粘贴
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <rect x="8" y="2" width="8" height="4" rx="1" stroke="#4A5568" stroke-width="2.5"/>
  <rect x="4" y="4" width="16" height="18" rx="3" stroke="#4A5568" stroke-width="2.5"/>
  <line x1="9" y1="13" x2="15" y2="13" stroke="#9FEDD7" stroke-width="2" stroke-linecap="round"/>
  <line x1="9" y1="17" x2="12" y2="17" stroke="#9FEDD7" stroke-width="2" stroke-linecap="round"/>
</svg>
```

### undo.svg - 撤销
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 3 7 L 3 3 L 7 3" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M 3 3 C 5 5 8 7 12 7 C 17 7 21 11 21 16 C 21 19 19 21 17 21" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

### redo.svg - 重做
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 21 7 L 21 3 L 17 3" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M 21 3 C 19 5 16 7 12 7 C 7 7 3 11 3 16 C 3 19 5 21 7 21" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

### refresh.svg - 刷新（静态）
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 3 12 C 3 7 7 3 12 3 C 16 3 19 5 21 8" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <path d="M 21 12 C 21 17 17 21 12 21 C 8 21 5 19 3 16" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <polyline points="17,3 21,3 21,7" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" fill="none"/>
  <polyline points="7,21 3,21 3,17" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" fill="none"/>
</svg>
```

### download.svg - 下载
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 3 17 L 3 19 C 3 20 4 21 5 21 L 19 21 C 20 21 21 20 21 19 L 21 17" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <polyline points="8,11 12,15 16,11" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" fill="none"/>
  <line x1="12" y1="3" x2="12" y2="15" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

---

## 设置/系统类

### settings.svg - 设置
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <circle cx="12" cy="12" r="8" stroke="#4A5568" stroke-width="2.5"/>
  <circle cx="12" cy="12" r="3" fill="#9FEDD7"/>
  <rect x="11" y="2" width="2" height="3" rx="1" fill="#4A5568"/>
  <rect x="11" y="19" width="2" height="3" rx="1" fill="#4A5568"/>
  <rect x="2" y="11" width="3" height="2" ry="1" fill="#4A5568"/>
  <rect x="19" y="11" width="3" height="2" ry="1" fill="#4A5568"/>
</svg>
```

### filter.svg - 筛选
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 4 4 L 20 4 L 14 12 L 14 20 L 10 18 L 10 12 Z" stroke="#4A5568" stroke-width="2.5" stroke-linejoin="round"/>
</svg>
```

### search.svg - 搜索
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <circle cx="10" cy="10" r="6" stroke="#4A5568" stroke-width="2.5"/>
  <line x1="15" y1="15" x2="20" y2="20" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

### help.svg - 帮助
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <circle cx="12" cy="12" r="10" stroke="#4A5568" stroke-width="2.5"/>
  <path d="M 9 9 C 9 7 10 6 12 6 C 14 6 15 7 15 9 C 15 10 14 11 12 11 L 12 13" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <circle cx="12" cy="17" r="1.5" fill="#4A5568"/>
</svg>
```

### info.svg - 信息
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <circle cx="12" cy="12" r="10" stroke="#4A5568" stroke-width="2.5"/>
  <circle cx="12" cy="8" r="1.5" fill="#4A5568"/>
  <line x1="12" y1="12" x2="12" y2="16" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

### warning.svg - 警告
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 10.3 3.7 L 2 18 C 1 19.7 2.2 22 4.2 22 L 19.8 22 C 21.8 22 23 19.7 22 18 L 13.7 3.7 C 12.8 2.1 11.2 2.1 10.3 3.7 Z" stroke="#4A5568" stroke-width="2.5" stroke-linejoin="round"/>
  <line x1="12" y1="9" x2="12" y2="13" stroke="#F4D06F" stroke-width="2.5" stroke-linecap="round"/>
  <circle cx="12" cy="17" r="1.5" fill="#F4D06F"/>
</svg>
```

### security.svg - 安全
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <rect x="5" y="11" width="14" height="10" rx="3" stroke="#4A5568" stroke-width="2.5"/>
  <path d="M 8 11 L 8 7 C 8 5 10 3 12 3 C 14 3 16 5 16 7 L 16 11" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <circle cx="12" cy="16" r="2" fill="#9FEDD7"/>
</svg>
```

### theme.svg - 主题
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <circle cx="12" cy="12" r="5" stroke="#4A5568" stroke-width="2.5"/>
  <path d="M 12 2 L 12 4 M 12 20 L 12 22 M 4 12 L 2 12 M 22 12 L 20 12 M 6 6 L 4.5 4.5 M 17.5 17.5 L 19 19 M 6 18 L 4.5 19.5 M 17.5 6.5 L 19 5" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <path d="M 12 7 A 5 5 0 0 1 12 17 Z" fill="#4A5568"/>
</svg>
```

---

## 文件/文档类

### file.svg - 文件
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 13 2 L 6 2 C 5 2 4 3 4 4 L 4 20 C 4 21 5 22 6 22 L 18 22 C 19 22 20 21 20 20 L 20 9 Z" stroke="#4A5568" stroke-width="2.5" stroke-linejoin="round"/>
  <polyline points="13,2 13,9 20,9" stroke="#4A5568" stroke-width="2.5" stroke-linejoin="round" fill="none"/>
</svg>
```

### folder.svg - 文件夹
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 4 20 L 4 6 C 4 5 5 4 6 4 L 10 4 L 12 6 L 20 6 C 21 6 22 7 22 8 L 22 18 C 22 19 21 20 20 20 Z" stroke="#4A5568" stroke-width="2.5" stroke-linejoin="round"/>
</svg>
```

### upload.svg - 上传
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 3 17 L 3 19 C 3 20 4 21 5 21 L 19 21 C 20 21 21 20 21 19 L 21 17" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <polyline points="8,9 12,5 16,9" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" fill="none"/>
  <line x1="12" y1="5" x2="12" y2="17" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

### attach.svg - 附件
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 21 10 L 11 20 C 9 22 6 22 4 20 C 2 18 2 15 4 13 L 14 3 C 15 2 17 2 18 3 C 19 4 19 6 18 7 L 9 16 C 8.5 16.5 7.5 16.5 7 16 C 6.5 15.5 6.5 14.5 7 14 L 15 6" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### image.svg - 图片
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <rect x="3" y="3" width="18" height="18" rx="3" stroke="#4A5568" stroke-width="2.5"/>
  <circle cx="8.5" cy="8.5" r="2" fill="#FF9D9A"/>
  <path d="M 3 15 L 7 11 L 12 16 L 16 12 L 21 17 L 21 19 C 21 20 20 21 19 21 L 3 21 Z" fill="#9FEDD7"/>
</svg>
```

### document.svg - 文档
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 14 2 L 6 2 C 5 2 4 3 4 4 L 4 20 C 4 21 5 22 6 22 L 18 22 C 19 22 20 21 20 20 L 20 8 Z" stroke="#4A5568" stroke-width="2.5" stroke-linejoin="round"/>
  <polyline points="14,2 14,8 20,8" stroke="#4A5568" stroke-width="2.5" stroke-linejoin="round" fill="none"/>
  <line x1="8" y1="13" x2="16" y2="13" stroke="#9FEDD7" stroke-width="2" stroke-linecap="round"/>
  <line x1="8" y1="17" x2="13" y2="17" stroke="#9FEDD7" stroke-width="2" stroke-linecap="round"/>
</svg>
```

---

## 状态/反馈类

### success.svg - 成功
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <circle cx="12" cy="12" r="10" stroke="#4A5568" stroke-width="2.5"/>
  <polyline points="7,12 10,15 17,8" stroke="#9FEDD7" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" fill="none"/>
</svg>
```

### error.svg - 错误
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <circle cx="12" cy="12" r="10" stroke="#4A5568" stroke-width="2.5"/>
  <line x1="8" y1="8" x2="16" y2="16" stroke="#FF9D9A" stroke-width="2.5" stroke-linecap="round"/>
  <line x1="16" y1="8" x2="8" y2="16" stroke="#FF9D9A" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

### loading.svg - 加载（静态）
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 12 3 A 9 9 0 0 1 21 12" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" fill="none"/>
  <circle cx="12" cy="3" r="2" fill="#FF9D9A"/>
</svg>
```

### favorite.svg - 收藏
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 12 2 L 15 9 L 22 10 L 17 15 L 18 22 L 12 18 L 6 22 L 7 15 L 2 10 L 9 9 Z" stroke="#4A5568" stroke-width="2.5" stroke-linejoin="round" fill="#F4D06F" fill-opacity="0.3"/>
</svg>
```

### like.svg - 点赞
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 12 21 C 12 21 3 14 3 9 C 3 6 5 4 7 4 C 9 4 11 5 12 7 C 13 5 15 4 17 4 C 19 4 21 6 21 9 C 21 14 12 21 12 21 Z" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round" fill="#FF9D9A" fill-opacity="0.3"/>
</svg>
```

### bookmark.svg - 书签
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 19 21 L 12 16 L 5 21 L 5 5 C 5 4 6 3 7 3 L 17 3 C 18 3 19 4 19 5 Z" stroke="#4A5568" stroke-width="2.5" stroke-linejoin="round"/>
</svg>
```

---

## 媒体控制类

### play.svg - 播放
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <circle cx="12" cy="12" r="10" stroke="#4A5568" stroke-width="2.5"/>
  <path d="M 10 8 L 16 12 L 10 16 Z" fill="#9FEDD7"/>
</svg>
```

### pause.svg - 暂停
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <circle cx="12" cy="12" r="10" stroke="#4A5568" stroke-width="2.5"/>
  <line x1="10" y1="8" x2="10" y2="16" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <line x1="14" y1="8" x2="14" y2="16" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

### stop.svg - 停止
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <circle cx="12" cy="12" r="10" stroke="#4A5568" stroke-width="2.5"/>
  <rect x="8" y="8" width="8" height="8" rx="1" fill="#FF9D9A"/>
</svg>
```

### volume.svg - 音量
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 11 5 L 6 9 L 2 9 L 2 15 L 6 15 L 11 19 Z" stroke="#4A5568" stroke-width="2.5" stroke-linejoin="round"/>
  <path d="M 15 9 C 16 10 17 11 17 12 C 17 13 16 14 15 15" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
  <path d="M 18 6 C 20 8 21 10 21 12 C 21 14 20 16 18 18" stroke="#4A5568" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

### mute.svg - 静音
```xml
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
  <path d="M 11 5 L 6 9 L 2 9 L 2 15 L 6 15 L 11 19 Z" stroke="#4A5568" stroke-width="2.5" stroke-linejoin="round"/>
  <line x1="23" y1="9" x2="17" y2="15" stroke="#FF9D9A" stroke-width="2.5" stroke-linecap="round"/>
  <line x1="17" y1="9" x2="23" y2="15" stroke="#FF9D9A" stroke-width="2.5" stroke-linecap="round"/>
</svg>
```

---

## 使用示例

**路径约定**：保存至本 skill 的 `resources/`（`.cursor/skills/generate-ai-icon/resources/<功能名称>.svg`），与 [SKILL.md](SKILL.md) 路径规范一致。

**批量生成**（从这个文件复制代码）：

```
用户："生成 10 个核心图标"

Agent 执行：
1. 读取 ICON-EXAMPLES.md
2. 从"核心导航类"和"消息/通信类"选择 10 个
3. 复制 SVG 代码
4. 使用 Write 工具保存到 .cursor/skills/generate-ai-icon/resources/<功能名称>.svg
```

**基于现有风格生成新图标**：

```
用户："生成一个翻译图标"

Agent 执行：
1. 读取本 skill 的 resources/ 中的现有图标（如 menu.svg）
2. 提取参数：stroke-width="2.5", stroke="#4A5568"
3. 设计翻译图标（如两个语言符号 A ↔ 文）
4. 编写 SVG 代码（使用相同参数）
5. 保存到 .cursor/skills/generate-ai-icon/resources/translate.svg
```
