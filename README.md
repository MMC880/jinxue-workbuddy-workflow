# 晋学智辅 · WorkBuddy 工作流包 v0.1.0

更新：2026-11-04。用户已选择 B 路线并授权搭建第一包。交付内容是操作规则、提示词、模板和虚构样例；尚未在 WorkBuddy 完成实测，不能直接用于真实学生归档。

## 从这里开始

1. 将本目录复制或解压到独立本地目录，在 WorkBuddy 桌面端选择该目录为工作空间；保持默认权限。不要选择上层磁盘或把整个目录上传云端资料库。
2. 复制 [START.md](START.md) 的区块到新任务。它会指引 WorkBuddy 先预检，再等待具体操作。
3. 查看 [环境预检表](checks/ENVIRONMENT.md)。UNKNOWN 必须保留未知，文件存在不等于工具可用。
4. 预检完成后，可按 [合成演练步骤](samples/synthetic/04_RUNBOOK.md)逐生演练。所有样例均虚构，没有真实身份映射。
5. 核对 [预期结果](samples/synthetic/05_EXPECTED_RESULTS.md)和[验收清单](checks/ACCEPTANCE.md)。预期结果不是已执行证据；WorkBuddy 必须记录自己的实际结果。

仅 START 中的预检是初次操作。其后按操作编号执行，不默认连跑全部步骤。老师的审核是业务动作，不需要每次生成草稿都重新批准开发。

## 项目边界

山西太原、目标 2027 年中考、现有十人再次备考班，内容目标为完整初中数学。学生完成老师布置的作业后，再由 AI 辅助整理；老师逐生看完整卷，确认问题后归档，随后汇总班级共性。给学生的讲解、练习与复测反馈均须先经老师审核。

每生积累学习问题、历史证据、当前表现与优势。一次答对不直接判掌握。心理档案、画像、诊断和人格标签完全排除。后续独立软件、会员、中转合作另阶段实施。

## 操作入口

| 操作 | 提示词 | 输出模板 |
| --- | --- | --- |
| 00 环境预检 | [预检](prompts/00_PREFLIGHT.md) | [环境表](checks/ENVIRONMENT.md) |
| 01 收件核对 | [收件](prompts/01_INTAKE.md) | [材料表](templates/INTAKE.md) |
| 02 逐生整卷分析 | [整卷](prompts/02_PAPER_ANALYSIS.md) | [整卷审核表](templates/PAPER_REVIEW.md) |
| 03 教师复核与拟归档 | [复核](prompts/03_REVIEW_ARCHIVE.md) | [档案变更单](templates/ARCHIVE_CHANGE.md) |
| 04 班级共性 | [汇总](prompts/04_CLASS_SUMMARY.md) | [班级摘要](templates/CLASS_SUMMARY.md) |
| 05 讲解、补练与按需导出 | [辅导](prompts/05_TUTORING_EXPORT.md) | [反馈与补练单](templates/TUTORING.md) |
| 06 复测更新 | [复测](prompts/06_RETEST.md) | [复测记录](templates/RETEST.md) |

共用规则：[工作流规则](rules/WORKFLOW_RULES.md)、[数据边界](rules/DATA_BOUNDARIES.md)。教师实际勾选与确认见 [教师复选表](checks/TEACHER_REVIEW.md)。依赖见 [能力说明](environment/CAPABILITIES.md)。结果目录见 [runs 约定](runs/README.md)。

## 版本与真实使用门槛

本包无自动执行脚本、数据库、网页或自动加载 Skill 配置。Markdown 勾选和提示词不构成安全隔离、事务或身份认证。真实档案更新仍需验证受限本地工具／人工管理路径，不能把完整档案读给模型来实现。

本版默认 `SYNTHETIC_ONLY`；真实试点需先验证授权、最小材料范围、模型与文件访问边界、文档公式质量、归档／恢复和净省时标准。不得由模型自行将模式改为 REAL。原电脑上的 Codex 技能及解释器路径没有随包迁移。
