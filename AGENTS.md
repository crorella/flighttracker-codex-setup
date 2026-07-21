# Repository guidance

## Scope

- Keep this repository limited to reusable Codex configuration for finding low-cost flight combinations.
- Write documentation and user-facing examples in clear, neutral language.
- Never commit booking references, traveler data, authentication material, or generated trip artifacts.

## Validation

- Validate the skill after editing `SKILL.md`.
- Validate the plugin after changing its manifest or packaged components.
- Review the complete Git diff for sensitive information before every push.

## Release expectations

- Keep the plugin manifest version in semantic-version format.
- Document user-visible installation changes in `README.md`.
