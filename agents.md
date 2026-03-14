# AGENTS.md

## Project goal
This repository is being localized into Simplified Chinese for a Chinese-language distribution.

## Scope
Only modify user-visible text and localization-related resources.
Do not change protocol fields, identifiers, class names, function names, enum values, log keys, or networking behavior unless explicitly asked.

## Localization rules
- Prefer resource-based localization over hardcoded text edits.
- Preserve technical abbreviations when necessary, such as CoT, ATAK, Plugin.
- Use Simplified Chinese (zh-CN).
- If a term is ambiguous, leave a TODO comment instead of guessing.

## Priority
1. Find all user-visible strings
2. Add/extend zh-CN localization resources
3. Refactor hardcoded UI strings into resources where safe
4. Report untranslated or ambiguous strings

## Expected outputs
- Clear summary of changed files
- Notes on uncertain translations
- Any build/test issues found
