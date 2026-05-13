# deepseek-v4 技术报告网站

>
> 
>
---

## 00、配置 Claude code + 安装 huashu-design

---

## 01、生成提示词

我想基于 Claude Code 和 Huashu-design（./.agents/skills/huashu-design），通过提示词将 deepseek-v4 的技术报告，转换成一个网页，网页内容可参考 .bing/website-index.html。

请给我简洁可用的提示词。

```markdown
请使用 huashu-design skill，将 DeepSeek-V4 技术报告（pdf/DeepSeek_V4-20260506.pdf）转换成一个高质量的中文网页。

## 设计参考
- 配色：DeepSeek 蓝(#4D6BFE)为主色，深蓝(#3A52D9)、浅蓝(#7E93FF)、蓝洗底(#EEF1FF)辅助
- 字体：Source Serif 4 (serif标题) + 系统字体 (正文) + JetBrains Mono (数据/标签)
- 风格：编辑式排版（editorial），衬线标题 + 高信息密度 + 克制留白

## 网页结构（按此顺序组织内容）
1. **导航栏**：DeepSeek logo + API文档/体验链接
2. **Hero区**：标题 + 副标题 + 核心数据（1M上下文、27%推理FLOPs、10% KV Cache）
3. **两个模型**：V4-Pro(旗舰) vs V4-Flash(高效) 参数对比卡片
4. **四项架构创新**：mHC残差 / CSA+HCA注意力 / Muon优化器 / FP4 QAT量化
5. **效率突破**：SVG曲线图(V3.2 vs V4 FLOPs对比) + 数据说明
6. **Benchmark对标**：与 Opus 4.7 / GPT-5.5 / Gemini 3.1 Pro 的成绩表
7. **诚实审视**：品味差/Agent短板/知识广度/本分姿态 四张卡片
8. **定价**：Pro 和 Flash 的人民币价格 + 对比闭源的价格优势
9. **生态适配**：Agent 框架兼容（Claude Code/OpenClaw/OpenCode/CodeBuddy）
10. **引语**：荀子「不诱于誉，不恐于诽」
11. **Footer**：DeepSeek 链接 + 版权

## 技术要求
- 单文件 HTML，所有 CSS inline
- 固定宽度 1280px，居中
- 不使用框架，纯 HTML+CSS
- SVG 内联绘制图表
- 输出到项目根目录 `index.html`

## 内容要求
- 从 PDF 技术报告中提取真实数据和原文
- 保持「花叔视角」的解读风格：坦诚、不吹、有观点
- 数据必须准确，不确定的标注「论文未披露」
```


---