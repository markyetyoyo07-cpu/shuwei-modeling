# 来源与资源

本技能为本次请求重新编写的数维杯辅助工作流，没有复制三个仓库的源码或角色手册，不代表三个项目维护者背书，也未经完整赛题效果测试。

参考设计：
- https://github.com/XiaoMaColtAI/math-modeling-skill ：复现清单、阶段产物检查与可回退版本。
- https://github.com/jihe520/MathModelAgent ：阶段化产物、排版和视觉检查。
- https://github.com/rootkiller6788/mathmodel-skill ：项目状态持久化、依赖关系与局部返工。

核查到的模板问题：https://github.com/jihe520/MathModelAgent/blob/main/skills/5writing/templates/zh/shuweibei-latex/main.tex 存在中文排版、旧届次和示例队号。它不适合作为2026秋季赛未经修订的模板。

官方资源核查日期2026-11-16；公开仓库仅提供下载链接与核查值，不重新分发资源。下列文件名是下载后的建议本地文件名，使用范围及内部版权声明遵循原发布者要求：

| 本地文件 | 来源 | SHA-256 |
|---|---|---|
| assets/official-2026-autumn-word.docx | https://www.nmmcm.org.cn/static/upload/file/20261110/1794283053784346.docx | 732db89498eb0dc6fe3d4ca08d9b21346ef95d14f1ee3d3b451debe49dbe7d5c |
| assets/official-2026-autumn-latex.zip | https://www.nmmcm.org.cn/static/upload/file/20261110/1794283053145164.zip | 53652fc1e88444ce9eeeebae9ed6e038d7c8e2a9517465667c6b5c72f28b1a3f |

LaTeX压缩包包含demo.tex、swmcmthesis.cls、swmcmthesis.cfg、示例图片和demo.pdf。已检查包目录及入口文本；本机未发现TeX编译器，未进行编译验证。附带demo.pdf是原发布者样例，不能作为本次编译成功证据。Word已检查可解析及正文内容，没有修改模板。
