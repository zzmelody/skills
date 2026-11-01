<!-- 生成说明：替换变量，删除本说明和无关章节。写当前项目的真实边界，不引入模板预设架构。不要链接其他 skill；支持文件放本 skill 内。 -->
---
name: {{PROJECT_SLUG}}-project-structure
description: {{STRUCTURE_DESCRIPTION_WITH_ACTUAL_SCOPE_AND_TRIGGERS}}
---

# {{PROJECT_NAME}} 项目结构规范

{{PROJECT_SCOPE_AND_CONFIRMED_TECHNICAL_CHOICES}}

## 规范独立性

本规范禁止依赖项目外的内容，不链接、调用或要求加载其他 skill，也不通过共享文档形成隐含依赖。补充规则保留在本 skill 目录内，内部文件可以互相引用。项目源码与配置可作为事实输入，不充当外置规范。

## 目录与模块职责

{{ACTUAL_DIRECTORY_RESPONSIBILITIES_AND_FILE_PLACEMENT}}

## 依赖与运行边界

{{ALLOWED_DEPENDENCY_DIRECTIONS_PUBLIC_INTERFACES_AND_PLATFORM_BOUNDARIES}}

## 技术方案与依赖管理

{{CONFIRMED_TOOLCHAIN_DEPENDENCY_OWNERSHIP_AND_CHANGE_CRITERIA}}

## 临时文件与正式产物

- Agent 的临时脚本、一次性工具、日志、截图、调试输出和下载物一律放项目根 `local/`，按需创建，可按任务建子目录。
- 禁止在源码、文档、规则目录或项目根散落写入临时文件。`local/` 随时可以整体删除，不保存需要保留或交付的内容。
- 源码、构建配置和正式文档不得引用或依赖 `local/`。需要长期保留的工具进入项目正式工具目录；正式交付文件使用约定的交付位置。
- 测试使用测试框架管理或系统隔离的临时目录并自行清理，不写真实用户存储，不依赖仓库 `local/`。
- 框架受管的构建产物和缓存沿用既有目录；用户明确指定的输出位置遵从本次指令。

{{LOCAL_IGNORE_STATUS_AND_FORMAL_TOOL_ARTIFACT_LOCATIONS}}

## 项目特有约束

{{ONLY_RELEVANT_DATA_CREDENTIAL_COMPATIBILITY_AND_COST_BOUNDARIES}}
