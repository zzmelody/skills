<!-- 生成说明：替换变量，删除本说明和无关章节。遵循真实配置；推荐但尚未落地的规则应明确状态。多语言细则可拆入本 skill 的 references，不链接其他 skills 或外部指南。 -->
---
name: {{PROJECT_SLUG}}-code-style
description: {{CODE_STYLE_DESCRIPTION_WITH_LANGUAGES_DIRECTORIES_AND_TRIGGERS}}
---

# {{PROJECT_NAME}} 代码规范

{{LANGUAGE_FRAMEWORK_DIRECTORY_SCOPE_AND_CONFIGURED_BASELINE}}

## 规范独立性

本规范禁止依赖项目外的内容，不链接、调用或要求加载其他 skill，也不通过共享文档形成隐含依赖。补充规则保留在本 skill 目录内，内部文件可以互相引用。项目源码与配置可作为事实输入，不充当外置规范。

## 格式与命名

{{EXISTING_FORMATTER_ENCODING_NAMING_AND_FILE_CONVENTIONS}}

## 语言与模块约定

{{APPLICABLE_TYPE_INTERFACE_IMPORT_EXPORT_AND_MODULE_RULES}}

## 错误、资源与副作用

{{RELEVANT_INPUT_VALIDATION_ERROR_HANDLING_RESOURCE_AND_ASYNC_RULES}}

## 框架约定

{{ONLY_APPLICABLE_FRAMEWORK_RULES_OR_INTERNAL_REFERENCES}}

## 实际可用的检查

{{VERIFIED_COMMANDS_WITH_WORKING_DIRECTORIES_SCOPE_AND_LIMITATIONS}}

{{RECOMMENDED_BUT_NOT_CONFIGURED_RULES_IF_ANY}}
