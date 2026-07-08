# 📚 Paper Analysis Reviewer Skill

这是一个用于 **深度学术论文分析** 的 ChatGPT Skill 仓库。Skill 名称为：

```text
paper-analysis-reviewer
```

它面向管理学、新闻传播学、出版学、人文社科与实证研究论文，帮助 ChatGPT 以 **严格但公正的学术审稿人 + 研究训练导师** 的方式阅读论文，而不是只做摘要复述。

## ✨ 这个 Skill 能做什么

`paper-analysis-reviewer` 适合用于：

- 🧭 判断论文类型：理论论文、实证论文、方法论文、综述论文、案例研究、人文社科解释性论文或混合类型论文
- 🔍 拆解真实问题意识：区分作者声称的问题与论文实际解决的问题
- 🧱 分析隐含假设：识别数据、方法、任务、实验、应用推广中的高风险前提
- 💡 判断真实创新点：说明创新到底发生在哪个理论、方法、证据或研究设计环节
- ⚠️ 寻找失效场景：提出反例、失败条件与结论边界
- 📝 生成审稿意见：输出主要质疑、次要质疑、作者回应路径与审稿倾向
- 🌱 提出后续研究方向：形成可继续发展的研究问题、数据方案与实验思路
- 📊 专项分析实证论文：检查变量、测量、模型、因果识别、稳健性与外部效度
- 🧠 专项分析人文社科论文：检查概念谱系、理论传统、材料证据、章节结构与语言逻辑

## 🎯 适用场景

这个 Skill 特别适合：

- 研究生、博士生做文献精读
- 写文献综述、开题报告、论文选题分析
- 训练 CSSCI / SSCI 风格的论文评价能力
- 对投稿论文进行预审稿
- 拆解人文社科论文的概念、论证与结构
- 检查实证论文是否存在因果推断、变量测量或模型设定问题

## 🗂️ 仓库结构

```text
literature-analysis-skill-repo/
├── README.md
├── requirements.md
├── codex_task_prompt.md
├── paper-analysis-reviewer/
│   ├── SKILL.md
│   ├── agents/
│   │   └── openai.yaml
│   └── references/
│       ├── review_templates.md
│       ├── empirical_paper_guide.md
│       └── humanities_social_science_guide.md
└── dist/
    └── skill.zip
```

## 🧩 核心文件说明

| 文件 | 作用 |
|---|---|
| `paper-analysis-reviewer/SKILL.md` | Skill 主说明文件，定义触发场景、工作流和输出规则 |
| `paper-analysis-reviewer/agents/openai.yaml` | Skill 在界面中的名称、简介和默认调用提示 |
| `references/review_templates.md` | 中文学术分析输出模板，包括简版、完整版、审稿意见与后续研究模板 |
| `references/empirical_paper_guide.md` | 实证论文专项检查框架 |
| `references/humanities_social_science_guide.md` | 人文社科论文专项检查框架 |
| `requirements.md` | 项目需求说明 |
| `codex_task_prompt.md` | 后续维护或扩展该 Skill 时可复用的 Codex 提示词 |
| `dist/skill.zip` | 可上传或导入的 Skill 压缩包 |

## 🚀 如何使用

如果你的 ChatGPT / Codex 环境支持导入 Skill，可以使用：

```text
dist/skill.zip
```

压缩包中包含完整的 `paper-analysis-reviewer/` Skill 目录，包括：

- `SKILL.md`
- `agents/openai.yaml`
- `references/` 下的三份专项参考文件

导入后，可以用类似下面的方式调用：

```text
请使用 paper-analysis-reviewer 分析这篇论文，重点判断它的真实问题意识、创新点、隐含假设、审稿风险和后续研究方向。
```

## 🧪 推荐分析方式

为了获得更好的分析结果，建议向 ChatGPT 提供以下材料：

- 论文标题
- 摘要
- 引言
- 理论假设或研究问题
- 方法与数据部分
- 结果与讨论
- 结论
- 如有可能，提供参考文献或作者声称对话的核心文献

如果只提供摘要，Skill 也会进行临时判断，但会明确标注不确定信息和需要进一步验证的路径。

## ✅ 输出风格

默认输出为中文，风格应当：

- 严格但公正
- 具体而非泛泛评价
- 不只复述摘要
- 明确区分事实、推断和不确定信息
- 给出可操作的修改建议和后续研究方向

## 🛠️ 如何继续迭代

如果要扩展这个 Skill，建议遵循以下原则：

1. 修改核心流程时，优先更新 `paper-analysis-reviewer/SKILL.md`
2. 添加详细模板、检查表或学科专项框架时，放入 `paper-analysis-reviewer/references/`
3. 保持 `SKILL.md` 简洁，避免把所有细节堆进主文件
4. 修改后重新打包 `dist/skill.zip`
5. 使用 Git 提交每一次稳定修改

常用命令：

```bash
git add .
git commit -m "update paper analysis reviewer skill"
git push
```

## 🌐 GitHub 版本管理

当前仓库可推送到 GitHub 进行版本管理。首次设置远程仓库时可使用：

```bash
git remote add origin git@github.com:<your-user>/<your-repo>.git
git push -u origin main
```

如果已经设置远程仓库，后续只需要：

```bash
git push
```

## 📌 设计原则

这个 Skill 的核心不是“帮用户总结论文”，而是帮助用户训练真正的论文判断能力：

- 这篇论文到底在解决什么问题？
- 它的创新是否真实存在？
- 它依赖哪些没有明说的前提？
- 它在哪些场景下会失效？
- 审稿人会如何质疑它？
- 它还能发展出什么新的研究问题？

简而言之，它是一个面向高阶学术阅读与论文训练的审稿式分析工具。
