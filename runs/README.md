# 演练输出目录约定

当前没有实际 WorkBuddy 运行记录，不预置“已通过”样例结果。

人工启动某次合成演练后，建议输出位于 `runs/SYN-RUN-001/`，内部按操作使用 intake.md、review-<student>.md、archive-proposals/、confirmed/、class-summary.md、tutoring/、retest/ 和 evidence.md。这些目录／文件按需生成，当前只是输出命名约定。

`confirmed/` 只用于虚构学生的人工模拟确认记录；真实档案不放在这里。每次输出记入操作号、源文件、mode、batch/student、状态和实际证据，不保留不必要的长对话。

重复演练先说明是复用同一 run_id 做重试，还是新建 run_id 做独立实验；不能为掩盖重复累计问题每次都换运行编号。覆盖已有结果前先保留历史版本；不修改样例／答案来凑预期。
