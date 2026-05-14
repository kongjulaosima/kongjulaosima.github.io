# 个人主页 - kongjulaosima.github.io

一个现代化的个人主页展示平台，包含多个独立页面模块，支持程序驱动的动画效果、论文学习和兴趣爱好分享功能。

## 项目结构

```
├── index.html          # 首页（主入口）
├── about.html          # 关于我
├── skills.html         # 技术技能
├── projects.html       # 项目展示
├── hobbies.html        # 个人兴趣爱好
├── papers.html         # 大模型论文学习
├── presentation.html   # HTML 演示文稿
├── deepseekV4.html     # DeepSeek V4 技术报告解读
├── contact.html        # 联系我
├── papers/              # 论文文件目录
│   ├── 2025.acl-long.11.pdf
│   ├── DeepSeek_V4.pdf
│   ├── deepseekV4技术点分析.pdf
│   ├── deepseekV4.docx
│   ├── StrucText-Eval.docx
│   └── StrucText-Eval.pptx
├── hobbies/            # 兴趣爱好资源目录
│   └── PUBG/           # PUBG 游戏截图
│       ├── pubg.md
│       └── *.jpg
└── prompts/           # 提示词文件
    └── prompt-make-website.md
```

## 页面预览

### 首页 (index.html)
- 粒子动画背景
- 打字机效果标题
- Glitch 故障艺术效果
- 3D 卡片悬停动画

### 关于我 (about.html)
- 个人简介展示
- 数据统计动画

### 技术技能 (skills.html)
- 技能卡片网格
- 涟漪点击效果

### 项目展示 (projects.html)
- 3D 变换项目卡片
- 标签系统

### 个人兴趣爱好 (hobbies.html)
- 游戏爱好展示卡片
- 浮动动画效果

### 大模型论文学习 (papers.html)
- PDF 论文展示卡片
- 在线阅读/下载功能
- 粒子交互背景

### DeepSeek V4 技术报告 (deepseekV4.html)
- DeepSeek-V4 技术报告中文解读
- DeepSeek 蓝品牌配色设计
- 模型架构创新展示
- 性能基准对比图表
- 开源生态兼容性说明

### HTML 演示文稿 (presentation.html)
- 幻灯片切换动画
- 键盘/触摸导航
- 进度条显示

### 联系我 (contact.html)
- 联系方式卡片

## 技术特性

- **纯前端实现** - 无需后端依赖
- **程序驱动动画** - Canvas 粒子系统、打字机效果、交互动画
- **响应式设计** - 适配各种屏幕尺寸
- **模块化结构** - 每个页面独立可运行

## 快速开始

直接用浏览器打开任意 `.html` 文件即可查看。

```bash
# 或者使用本地服务器
python -m http.server 8000
# 然后访问 http://localhost:8000
```

## 自定义修改

1. **修改个人信息** - 编辑各 `.html` 文件中的文本内容
2. **添加论文** - 将 PDF 文件放入 `papers/` 目录，并在 `papers.html` 中添加卡片
3. **添加游戏截图** - 将截图放入 `hobbies/PUBG/` 目录，并更新 `hobbies.html` 中的引用
4. **添加新的兴趣爱好** - 在 `hobbies/` 下创建新的子目录，并在 `hobbies.html` 中添加对应的展示区域
5. **修改样式** - 编辑各文件中的 `<style>` 标签
6. **添加新页面** - 复制现有页面模板，修改内容和导航链接
7. **创建新的技术报告解读** - 参考 `deepseekV4.html` 的模式，使用 huashu-design skill 创建新的技术报告页面

## 技术栈

- HTML5
- CSS3 (动画、Flexbox、Grid)
- JavaScript (Canvas API、Intersection Observer)
- 无外部依赖，纯原生实现

---

&copy; 2026 Built with ❤️
