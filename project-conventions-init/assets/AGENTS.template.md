<!-- 生成说明：这是骨架。替换变量并删除本说明，按项目规模裁剪。GLOBAL_RULES_ENTRY 仅生成项目全局规范的相对链接及必要触发条件；没有独立 skills 时，内联必要细则。不得链接专用 skills、局部指引或项目外内容。 -->
# {{PROJECT_NAME}} 工作区规则

{{PROJECT_PURPOSE_AND_SHAPE}}

{{ESSENTIAL_RUNTIME_AND_COMMAND_LOCATION}}

## 项目全局规范

{{GLOBAL_RULES_ENTRY}}

## 始终生效的约束

- 本文件与项目规范禁止依赖项目外的内容；skills 之间不得互相依赖，每个 skill 的支持文件保留在自身目录内。
- Agent 临时文件统一放项目根 `local/`；测试使用隔离临时目录并自行清理。
{{PROJECT_CRITICAL_CONSTRAINTS}}
