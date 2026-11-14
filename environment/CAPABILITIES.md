# 依赖与目标环境说明

本包只有 Markdown，不带程序、可执行 Skill、Python 环境、字体或数据库，不自动加载宿主配置。移动目录后仍按相对路径读取。

| 能力 | 已知情况 | WorkBuddy 当前结论 |
| --- | --- | --- |
| Markdown 读写 | 包已提供文本规则与模板 | 未实测 |
| 图片／手写数学 | 初包未提供真实图片样例 | 未实测；文本占位不证明 OCR |
| Word／PDF 读取生成 | 有规范和导出检查要求，未附转换引擎 | 未实测 |
| 精确代数核验 | 研发侧 Codex 已安装 K-Dense sympy Skill，并在独立环境核过六个自编表达式 | 不能据此视为 WorkBuddy 可调用；不要引用原电脑绝对解释器路径 |
| 本地写档、重复控制、恢复 | 有规则和验收场景 | 无确定性写档工具，真实数据未启用 |
| 访问／外发隔离 | 有既定业务边界 | 需要宿主权限和实际传输检查，提示词不能证明 |

若已有合适工具，先记录来源、版本和能实际执行的操作；若缺失，再按具体缺口用 find-skills 搜索 GitHub，核对许可、依赖、读写／外发范围，不在预检时自动下载。SymPy 是代数核验组件，不是识图、教学诊断或全题型证明判定器。

官方能力依据仅作研究参考，不是本机实测结果：[Skills](https://www.workbuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Function-Description/Skills-Market)、[项目与资料库](https://www.workbuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Function-Description/Project)、[权限](https://www.workbuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Function-Description/Permission-Modes)。文档可能变化，以届时实际环境核对为准。
