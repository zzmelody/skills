<!-- 生成说明：替换变量，删除本说明和无关章节。使用项目真实测试体系，不预设框架或强制为小改动补测试。不链接其他 skills；必要规则在本 skill 内完整表达。 -->
---
name: {{PROJECT_SLUG}}-testing
description: {{TESTING_DESCRIPTION_WITH_ACTUAL_SCOPE_AND_TRIGGERS}}
---

# {{PROJECT_NAME}} 测试与验证规范

{{ACTUAL_TEST_FRAMEWORK_AND_AVAILABLE_VERIFICATION_CAPABILITIES}}

## 规范独立性

本规范禁止依赖项目外的内容，不链接、调用或要求加载其他 skill，也不通过共享文档形成隐含依赖。补充规则保留在本 skill 目录内，内部文件可以互相引用。项目源码与配置可作为事实输入，不充当外置规范。

## 测试位置与写法

{{ACTUAL_TEST_LOCATIONS_NAMING_FIXTURES_AND_BEHAVIOR_CONVENTIONS}}

## 验证范围

- 根据行为变化和风险选择聚焦验证，关注可观察行为与真实失败路径，不写只复述实现的测试。
- 优先检查受影响范围，有跨模块影响或项目门禁要求时再扩大；通过后不无故重复全量检查。
- 调试、复现 bug 和阶段性验证按实际需要执行，不设置开发过程中禁止测试的规则。

{{PROJECT_SPECIFIC_COVERAGE_AND_REQUIRED_CHECKS}}

## 隔离、临时文件与外部依赖

- 测试使用框架管理或系统隔离的临时目录，注册清理，不依赖执行顺序、仓库 `local/` 或真实用户数据。
- 测试创建的进程、服务器、订阅、连接和定时器按项目框架机制释放。
- 测试之外的 Agent 临时脚本、日志、截图、调试输出和下载物放项目根 `local/`；正式交付文件与框架受管产物遵循各自约定。

{{RELEVANT_EXTERNAL_SERVICE_CREDENTIAL_COST_AND_ENVIRONMENT_GATES}}

## 检查命令与交付记录

{{VERIFIED_COMMANDS_WITH_WORKING_DIRECTORIES_AND_WIDENING_CRITERIA}}

只报告实际执行的结果。未运行、条件跳过、失败和通过分别说明；失败给出相关输出与影响，不把静态核对或合成样本当作真实集成验证。

{{DOCUMENTATION_UPDATE_REQUIREMENTS_AND_MISSING_CAPABILITIES_IF_ANY}}
