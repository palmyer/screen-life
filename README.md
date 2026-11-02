# 屏幕人生

每天看手机的时长无感，乘以已活天数就是触目惊心的数字

> 点子来源：Obsidian《人生可视化 / 屏幕人生》 · 同系列仓库参考 [life-grid](https://github.com/palmyer/life-grid)

## 功能

- 日均屏幕时长 + 开始使用年龄
- 已花年数 / 余生照旧还要花几年
- 换算锚点：相当于读完多少本书、看完多少部电影
- 赎回模拟器：每天少玩 30 分钟，余生能赎回多少个月

## 运行

纯静态零依赖，任选其一：

```bash
cd screen-life
python -m http.server 8740
```

- 网页版：<http://127.0.0.1:8740/>
- 手机壳预览：<http://127.0.0.1:8740/preview.html>（life-grid 同款）

或直接双击 `index.html`。

## 设计

- iOS 暗色风格：纯黑背景、#1C1C1E 分组卡片、SF 系统色板
- 选择一律使用 iOS 风格底部滚轮（`shared/wheel.js`）
- 数据存于浏览器 localStorage（`lv-` 前缀），不上传任何服务器
- 生日 / 预期寿命与同系列工具共享同一份配置
