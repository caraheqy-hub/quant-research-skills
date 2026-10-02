# Cara 的 Codex 技能清单与对照

核对时间：2026-10-02。这里的“已有”分为个人目录中已安装、系统内置和插件当前可用；插件技能不等于已复制到个人目录。技能是工作方法与操作提示，不是行情数据、交易接口或有效策略的保证。

## 个人目录中的技能

| 技能 | 来源与用途 | 当前判断 |
| --- | --- | --- |
| `project-craft` | 自写；项目先构想、查技能和开源、做最小清晰实现、核实后交付 | 已补公开发布前的凭证、个人路径、数据许可检查；适用于后续较大项目 |
| `factor-mining` | 自写；研报来源、公式、数据可得时点、因子实验与交易约束 | 已补受限研报/行情的分享边界；适用于因子、择时和选股研究 |
| `debug-ledger` | 自写；复现、追根、验证、记录可检索的错题本 | 新安装；把本次及历史上已观察的问题分类记录，未确诊问题不写成结论 |
| `skill-garden` | 自写；每次较大项目开始查适用技能，结束时分类经验、审查是否迭代 | 新安装；避免把单次事实、重复规则和未经证实的想法都塞进技能 |
| `source-research` | 自写；跨来源网页调查、原文核对、证据地图与停止条件 | 新安装；用于真正需要多来源综合的调查 |
| `bilingual-writing` | 自写；中英文“研究逻辑”和“克制的文采”两种改写模式 | 新安装；保留原事实、数字和引用，不编造经历 |
| `juejinquant` | 第三方 [fadewalk 项目](https://github.com/fadewalk/juejinquant-skill)；GM API 线索和示例 | 已安装，但接口以掘金官方文档和实际 SDK 为准；示例有一次确认的名称遮蔽问题；原项目声明限制商用，因此不把内容上传到自己的公开仓库 |
| `jupyter-notebooks` | 已安装的外部技能；可重跑的 Python/SQL 笔记 | 需要探索或审计轨迹时再用；QR 框架本身以命令行和 CSV/JSON 结果为准 |

## 系统内置与当前插件技能

| 名称 | 功能 | 使用时机 |
| --- | --- | --- |
| `imagegen` | 生成或编辑位图 | 真需要图片素材时 |
| `openai-docs` | OpenAI/Codex 官方产品文档 | 询问 Codex、API、模型和配置时 |
| `skill-creator` / `skill-installer` | 创建、校验或安装技能 | 新增和维护个人技能时 |
| `computer-use:computer-use` | 操作电脑界面 | 必须检查网页或桌面 UI 时 |
| `documents:documents` | Word 文档制作和检查 | `.docx` 交付时 |
| `pdf:pdf` | PDF 阅读、制作和版面检查 | 原文 PDF 或报告交付时 |
| `google-drive:google-drive` | Google Drive 文件入口 | 使用连接的云端文件时 |
| `google-drive:google-docs` / `google-drive:google-drive-comments` | Google 文档编辑、评论 | 对应原生文档时 |
| `google-drive:google-sheets` / `google-drive:google-slides` | Google 表格和幻灯片 | 对应原生文件时 |
| `spreadsheets:Spreadsheets` / `spreadsheets:excel-live-control` | 表格文件制作或活动 Excel 控制 | 表格交付或直播 Excel 会话时 |
| `presentations:Presentations` | 演示文稿 | 面试展示 deck 等任务时 |
| `public-equity-investing:public-equity-investing` | 上市公司、财报、估值、投资论证和组合风险路由；插件内含 23 个专门流程 | 做财报、基本面、研究报告和组合风控时；按问题调用相应流程，不复制一整套 |
| `plugin-management:plugin-management` | 外部插件发现和管理 | 缺数据连接或专门服务时 |
| `sites:sites-building` / `sites:sites-hosting` / `sites:sites-mcp` / `sites:sites-preview-troubleshooting` | Sites 建站、托管、MCP、预览排障 | 选择 Codex Sites 时；本次明确选择 GitHub Pages，因此未用它部署 |
| `template-creator:template-creator` | 可复用文档/演示/表格模板技能 | 用户要制作模板时 |
| `visualize:visualize` | 对话内交互可视化 | 因果、方案比较需要图形时 |
| `work-pets:create-pet` / `work-pets:pets` / `work-pets:update-pet` | ChatGPT Work 动画宠物 | 与量化项目无关，保持可用即可 |

`public-equity-investing` 插件的相关专门流程含财务报表口径与勾稽、三表、业绩前瞻/复盘、公司速览、可比估值、DCF、投资想法与多空论证、组合风险、催化剂日历。它们提供分析步骤，不自动带来券商研报全文、点时行情、企业授权数据或可交易收益。

## 和 GitHub 上相近项目的比较

| 公开资源 | 可借鉴的强项 | 对照后采取的动作 |
| --- | --- | --- |
| [obra/superpowers：系统排障](https://github.com/obra/superpowers/blob/main/skills/systematic-debugging/SKILL.md)与[交付前验证](https://github.com/obra/superpowers/blob/main/skills/verification-before-completion/SKILL.md) | 先查证据和根因，验证原故障消失 | 增加 `debug-ledger`，让错误案例可重用；未照搬其强制的长流程，保持按风险选择检查 |
| [quantskills/skill-quant-research](https://github.com/quantskills/skill-quant-research/blob/main/SKILL.md) | 点时数据、成本、回测纪律 | `factor-mining` 已覆盖基础研究口径；真实全市场点时股票池、停牌/涨跌停与容量模型仍是数据和工程缺口，不能靠技能文字补齐；该项目为 GPL，未复制内容 |
| [OpenAI Public Equity Investing 插件](https://github.com/openai/plugins/blob/main/plugins/public-equity-investing/README.md) | 财报、估值、组合风险等细分工作流 | 当前插件已可用，按任务调用；不再安装重名技能造成重复 |
| [Anthropic financial-services](https://github.com/anthropics/financial-services) | 金融分析工作流与连接器范例 | 一些流程依赖专有连接器/数据；当前项目不引入无法验证或无授权的数据依赖 |
| [fadewalk/juejinquant-skill](https://github.com/fadewalk/juejinquant-skill) | GM API 字典及使用线索 | 保留本地安装供查阅；例子需代码审查，接口需核对官方文档；不重新发布其文本 |
| [obra/superpowers 的 writing-skills](https://github.com/obra/superpowers/blob/main/skills/writing-skills/SKILL.md)和 [Anthropic skill-creator](https://github.com/anthropics/skills/blob/main/skills/skill-creator/SKILL.md) | 技能触发词、按需读取引用、更新后验证 | `skill-garden` 借鉴“技能也应迭代”的思路；缩小到可观察经验与简短场景检查，避免每次项目进行沉重的全库评测 |
| [REPOZY token-efficiency](https://github.com/repozy/superpowers-optimized/blob/main/skills/token-efficiency/SKILL.md) | 批处理、少重复、缩短常驻文本 | 不直接安装其全局常驻规则；`skill-garden` 采用按需加载、窄搜索和停止条件，保留必要查证与测试 |
| [dandaka deep-research](https://github.com/dandaka/skills/blob/main/deep-research/SKILL.md)和 [OpenAI 产品研究技能](https://github.com/openai/plugins/blob/main/plugins/product-design/skills/research/SKILL.md) | 多来源、交叉核对、综合 | 前者依赖 Exa 与并行代理，后者面向产品体验；`source-research` 保留通用的证据地图和原文核对，直接使用现有网页工具 |
| [blader/humanizer](https://github.com/blader/humanizer)、[中文论文写作技能](https://github.com/Findddx/codex-cn-paper-skills)、[Academic-paper-writing-skill](https://github.com/CarrieX6/Academic-paper-writing-skill) | 英语自然改写、中文学术论证和中英研究文稿 | 均有可取方法，但各自只覆盖部分场景；`bilingual-writing` 合并为两个明确模式，研究文本优先证据与逻辑，文艺表达按请求使用；未复制其文本 |

## 仍需要真实资源而非更多技能的部分

1. 全 A 股历史可投资股票池、公告点时基本面、真实可交易性与成本数据。没有它们，当前小样本结果只能是研究流程演示。
2. 最新券商研报要逐篇核实原文、发布日期、公式和使用权限。资料库中“线索”不等于“已复现”。
3. 在补齐数据后，再做行业/市值暴露、容量与组合风险、滚动样本外验证；随后扩展机器学习。当前无需为了技能数量安装不可靠的包。

## 项目文件位置

| 文件夹 | 内容 |
| --- | --- |
| `qr_factor_lab/` | 可运行的 A 股因子研究代码；`src/` 是程序，`tests/` 是 6 个时点与计算测试，`research/` 是 19 份研报与 34 个候选索引，`reports/` 和 `results/` 是一项公式复现及探索结果 |
| `qr_factor_lab/data/` | 本地掘金行情与来源记录；受许可约束，Git 忽略；公开版可用 `demo-data` 生成合成样本 |
| `quant-research-skills/` 内的六个技能文件夹 | 自写技能；其中 `debug-ledger/references/cases.md` 是错题本。前三个技能在 `outputs/` 还保留了单独的本地副本 |
| `cara-he-research-7954eefd5d4c1e7c/` | 静态求职网页，`index.html`、`styles.css`、`robots.txt`，以 GitHub Pages 发布 |
| `quant-research-skills/` | 六个自写技能的公开仓库副本和使用说明 |

原始行情、私有凭证和完整简历不在公开仓库。网页用随机项目路径和 `noindex` 降低偶然发现的概率，但 GitHub Pages 页面及公开仓库仍可被任何知道地址的人访问。
