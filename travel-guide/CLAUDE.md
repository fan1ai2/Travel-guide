# travel-guide — 城市旅游攻略

纯静态 HTML/CSS 落地页，面向自由行用户的六大热门城市旅游指南。

## 项目信息

- **名称**: 城市旅游攻略 2026
- **定位**: 热点城市自由行指南 — 让你的旅行更简单
- **覆盖城市**: 北京、上海、广州、成都、西安、杭州
- **目标用户**: 国内自由行旅客
- **Canonical URL**: `https://travel-guide.example.com/`

## 技术栈

- 纯 HTML5 + CSS3（无框架、无构建工具）
- 无 JavaScript 依赖（纯静态展示）
- 开发服务器：`python3 -m http.server 8080`

## 目录结构

```
travel-guide/
├── index.html          # 主页面（27KB，包含所有城市内容）
├── cities/             # 各城市子页面
├── css/
│   └── style.css       # 全局样式
├── robots.txt
└── sitemap.xml
```

## SEO 要求

- 每个城市页面有独立 title/description/keywords
- sitemap.xml 保持更新
- canonical URL 正确指向
- Open Graph 标签完整（title/description/image）
- 结构化数据（Schema.org Article/BreadcrumbList）

## 设计规范

- 移动优先，320px 起适配
- 图片懒加载，WebP 格式优先
- 无外部字体依赖，使用系统字体栈
- 颜色方案：清新旅行风（蓝绿色系为主色调）

## 部署

部署到 Nginx 静态托管，构建产物直接推送到 GitLab。
