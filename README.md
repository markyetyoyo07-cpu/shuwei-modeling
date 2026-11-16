# 数维杯建模协作 Skill

面向数维杯备赛与参赛的 Codex / Claude Code 辅助工作流：核对当届规则，整理队员方案和实验记录，建立结论与结果的对应关系，完成英文论文排版和交付核验。

当前包含2026秋季赛的规则参考和官方模板下载指引。其他年份、春季赛或不同报名入口需要重新核对，不能直接套用时间和格式。

## 能做什么

- 赛前检查官方模板、环境与 PDF 导出链路。
- 整理选题依据、附件、队员方案和子问题依赖。
- 保存结果来源、输入哈希、运行命令、环境和参数。
- 维护项目进度，跨会话恢复，只返工受影响的内容。
- 建立“论文主张—数值—结果字段—生成命令”的证据记录。
- 辅助翻译、润色、常规绘图、引用与逐页版式检查。
- 维护 AI 使用台账和提交前核对记录，保留可回退版本。

## 工作流

赛前环境与模板试跑 → 选题与队员方案 → 实验记录 → 验证与证据整理 → 英文论文 → 终审与提交。

只需要单个阶段时，可直接执行相应阶段。图表数量由证据和页数预算决定，不要求凑固定数量。

核心假设、模型构建、算法设计与求解、结果解释和结论由参赛队员自主完成。本技能按照2026年11月发布的官方 AI 规定安排辅助工作，不承诺获奖或检测比例。

## 安装

将仓库克隆或下载到技能目录，文件夹名称保持为 `shuwei-modeling`。

Codex 示例：

```bash
git clone https://github.com/markyetyoyo07-cpu/shuwei-modeling.git ~/.codex/skills/shuwei-modeling
```

Claude Code 示例：

```bash
git clone https://github.com/markyetyoyo07-cpu/shuwei-modeling.git ~/.claude/skills/shuwei-modeling
```

也可以下载 ZIP，解压后将包含 `SKILL.md` 的整个文件夹复制到上述位置。在新聊天中使用技能。

## 使用

Codex 示例：

```text
使用 $shuwei-modeling。先确认我的数维杯届次和当前官方规则，
检查环境与论文模板，建立参赛计划和 AI 使用台账。
核心模型由我们队伍独立设计，请辅助整理、核验、绘图和排版。
```

建议从题目项目目录启动，提供报名页面、队号、分工、题目和附件路径。项目产物写入题目目录，不写回技能目录。

## 文件说明

| 文件 | 用途 |
|---|---|
| [SKILL.md](SKILL.md) | 技能入口与阶段路由 |
| [参赛流程方案](参赛流程方案.md) | 分工、四天排期和检查节点 |
| [规则参考](references/2026-autumn.md) | 2026秋季赛规则入口与待澄清事项 |
| [执行契约](references/workflow.md) | 项目状态、证据字段和验收方式 |
| [来源说明](references/sources.md) | 设计参考、模板下载地址与哈希 |
| [模板下载指引](assets/README.md) | 官方 Word 与 LaTeX 模板链接及校验值 |

## 环境与验证

技能本身是 Markdown 指令和参考文件，无常驻服务。执行具体任务时按需准备 Python、Word 或 LaTeX、PDF 检查和绘图工具。使用官方模板时先在题目目录复制一份，清理示例内容并实际导出。

已通过技能 frontmatter、参考路径、元数据和资源哈希检查，并进行旧模板误用与临近截止返工的情境验证。尚未进行完整赛题效果基准测试；发布时未在本机编译官方 LaTeX 模板，仓库内 demo.pdf 是官方原包的示例，不是本项目编译验证成果。

## 设计参考

本项目重新编写工作流，参考了以下项目的设计，没有打包它们的完整代码或角色手册，也不依赖同时安装三个项目：

- [XiaoMaColtAI/math-modeling-skill](https://github.com/XiaoMaColtAI/math-modeling-skill)：复现记录、阶段检查与可回退版本。
- [jihe520/MathModelAgent](https://github.com/jihe520/MathModelAgent)：模块化产物、排版与视觉检查。
- [rootkiller6788/mathmodel-skill](https://github.com/rootkiller6788/mathmodel-skill)：状态恢复与局部返工。

## 官方依据

规则核查日期：2026年11月16日。正式使用前核对后续通知。

- [日程与报名通知](https://www.nmmcm.org.cn/News/198.html)
- [论文格式规范](https://www.nmmcm.org.cn/static/upload/file/20261105/1793866912597536.pdf)
- [AI 工具使用规定](https://www.nmmcm.org.cn/News/220.html)
- [官方模板发布页](https://www.nmmcm.org.cn/News/218.html)

## 许可

原创技能文本和项目文档采用 [MIT License](LICENSE)。仓库不重新分发第三方官方模板；自行下载的模板及其内部素材遵循原权利人声明，详见 [第三方资源说明](THIRD_PARTY_NOTICES.md)。本项目非赛事官方出品。
