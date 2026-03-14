# AGENTS.md

## Project objective
This repository is being localized into Simplified Chinese (zh-CN) for a Chinese-language distribution.

## Scope
Focus on user-visible localization work only.

Allowed:
- Add or extend zh-CN Android resource directories
- Translate user-visible strings in XML resource files
- Refactor clearly user-visible hardcoded UI strings into resources
- Report ambiguous terms and skipped items

Not allowed unless explicitly requested:
- Modify protocol fields
- Modify identifiers, class names, function names, enum values
- Modify log keys or behavior-sensitive constants
- Change networking, serialization, or plugin interfaces
- Translate non-translatable values or backing values in arrays.xml

## Repository priorities
1. atak/ATAK/app
2. plugin-examples modules that are actually user-facing
3. test/demo modules last

## Localization rules
- Use Simplified Chinese (zh-CN), not Traditional Chinese.
- Do not overwrite or alter existing values-zh-rTW resources unless explicitly requested.
- Prefer resource-based localization over direct inline string edits.
- Preserve technical abbreviations where appropriate, including:
  - ATAK
  - CoT
  - Plugin
- If a term is ambiguous, preserve English and add a TODO note.

## Glossary
- Situational Awareness = 态势感知
- Overlay = 图层
- Layer = 图层
- Marker = 标记点
- Route = 路线
- Track = 轨迹
- Geofence = 电子围栏
- Data Package = 数据包
- Plugin = 插件
- Mission = 任务
- Credential = 凭据
- Repository = 仓库
- Sync = 同步
- Grid = 网格
- Toolbar = 工具栏
- Preferences = 偏好设置
- CoT = CoT

## Arrays and XML rules
- In arrays.xml, only translate user-visible labels.
- Do not translate machine-readable values, IDs, keys, codes, or backing values.
- In preference/layout XML, replace hardcoded user-visible literals with @string references where safe.

## Output requirements
For every task, provide:
- files changed
- why each file was changed
- unresolved terminology
- skipped ambiguous strings
- build/test results if any were run
