# 00 环境预检

读取 [工作流规则](../rules/WORKFLOW_RULES.md)、[数据边界](../rules/DATA_BOUNDARIES.md)和[环境表](../checks/ENVIRONMENT.md)。本步骤不写文件、不执行终端、不读取秘密配置，不安装或调用外部服务做额外测试。

报告实际工作空间；从界面或已有获准状态核实 Markdown、图片、Word/PDF、数学核验与受限文件操作能力。看不到版本、权限或接口就标 UNKNOWN；不能根据工具名称、SKILL.md 存在或研发侧结果填 PASS。

输出填好的环境表到对话，说明每项依据和证据层级。指出真实数据的文件访问／外发隔离尚未完成，模式维持 SYNTHETIC_ONLY。

结束提示用户：下一步可按 [合成演练步骤](../samples/synthetic/04_RUNBOOK.md)启动 01。不要自动读取全部样例或运行后续业务。
