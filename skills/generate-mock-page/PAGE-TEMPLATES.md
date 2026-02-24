# 页面模板参考

生成模拟页面时按功能类型选择对应模板结构。

---

## 1. 表单页 (form)

**适用**：登录、注册、设置、单表单提交

```html
<main style="max-width: 400px; margin: 0 auto;">
  <h1>页面标题</h1>
  <form id="mainForm" onsubmit="return handleSubmit(event)">
    <label>输入项 1 <input type="text" required></label>
    <label>输入项 2 <input type="password" required></label>
    <button type="submit">提交</button>
  </form>
  <p><a href="#">次要操作链接</a></p>
</main>
<script>
  function handleSubmit(e) {
    e.preventDefault();
    alert('提交成功（模拟）');
    return false;
  }
</script>
```

**变体**：登录（邮箱+密码+记住+忘记密码）、注册（多字段+协议勾选）、设置（分组字段+保存）

---

## 2. 列表+详情 (list-detail)

**适用**：订单列表、用户列表、商品管理

```html
<main>
  <section class="toolbar">
    <input type="search" placeholder="搜索">
    <select><option>全部状态</option></select>
    <button>新增</button>
  </section>
  <section class="list">
    <article class="item" onclick="showDetail(1)">
      <span>项 1</span><span>状态</span>
    </article>
    <article class="item" onclick="showDetail(2)">...</article>
  </section>
  <div id="detailPanel" class="detail-panel" style="display:none">
    <h3>详情</h3>
    <p>字段1: xxx</p>
    <button onclick="closeDetail()">关闭</button>
  </div>
</main>
```

**变体**：左侧列表 + 右侧详情；表格 + 行点击展开；弹窗详情

---

## 3. 仪表盘 (dashboard)

**适用**：数据概览、统计指标

```html
<main>
  <section class="cards">
    <div class="card"><span class="value">1,234</span><span>指标1</span></div>
    <div class="card"><span class="value">56</span><span>指标2</span></div>
  </section>
  <section class="chart-placeholder">
    <div style="height:200px;background:#f0f0f0;display:flex;align-items:center;justify-content:center;border-radius:8px">
      图表区域（模拟）
    </div>
  </section>
</main>
```

---

## 4. 多步骤流程 (wizard)

**适用**：下单流程、配置向导

```html
<main>
  <nav class="steps">
    <span class="active">步骤1</span> → <span>步骤2</span> → <span>步骤3</span>
  </nav>
  <section id="step1">
    <h2>步骤 1</h2>
    <form>...</form>
    <button onclick="goStep(2)">下一步</button>
  </section>
  <section id="step2" style="display:none">...</section>
</main>
<script>
  function goStep(n) {
    document.querySelectorAll('section[id^="step"]').forEach(s => s.style.display = 'none');
    document.getElementById('step'+n).style.display = 'block';
  }
</script>
```

---

## 5. Tab 切换

**适用**：设置多 Tab、个人中心

```html
<main>
  <nav class="tabs">
    <button class="active" onclick="switchTab(1)">Tab1</button>
    <button onclick="switchTab(2)">Tab2</button>
  </nav>
  <div id="tab1" class="tab-content">内容 1</div>
  <div id="tab2" class="tab-content" style="display:none">内容 2</div>
</main>
```

---

## 6. 弹窗 (modal)

**适用**：确认删除、编辑表单弹窗

```html
<button onclick="document.getElementById('modal').style.display='flex'">打开弹窗</button>
<div id="modal" style="display:none;position:fixed;inset:0;background:rgba(0,0,0,0.5);align-items:center;justify-content:center;">
  <div style="background:white;padding:24px;border-radius:8px;max-width:400px;">
    <h3>弹窗标题</h3>
    <p>内容</p>
    <button onclick="document.getElementById('modal').style.display='none'">关闭</button>
  </div>
</div>
```

---

## 通用样式片段

```css
:root {
  --primary: #4A5568;
  --accent: #FF9D9A;
  --bg: #f8f9fa;
  --radius: 8px;
}
body { font-family: system-ui, -apple-system, sans-serif; margin: 0; padding: 24px; background: var(--bg); }
button {
  background: var(--primary); color: white; border: none; padding: 10px 20px;
  border-radius: var(--radius); cursor: pointer;
}
button:hover { opacity: 0.9; }
input, select { padding: 8px 12px; border: 1px solid #ddd; border-radius: var(--radius); }
```

---

## 与 generate-ai-icon 协同

页面中引用图标示例：

```html
<img src="../../.cursor/skills/generate-ai-icon/resources/menu.svg" alt="菜单" width="24" height="24">
```

或复制图标到 `mock-pages/<功能名>/assets/` 后相对路径引用。
