# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is an AI prompts repository containing structured prompts for various use cases. The repository is organized with prompts stored in the `prompts/` directory. Each prompt uses XML-structured formatting for clarity and consistency.

## Repository Structure

- `/prompts/` - Contains structured prompt files
- `.mise.toml` - Dependency management (requires `mise trust` and `mise install` on first use)
- `README.md` - Human-readable documentation
- `CLAUDE.md` - This file (AI assistant instructions)

## Working with Prompts

### Standard XML Structure Template

When creating or editing prompts, use this structure:

```xml
<role>
Define the AI's expertise, experience level, and domain knowledge
</role>

<context>
Provide background information and current state of the field
</context>

<instructions>
Clear, actionable directives for what the AI should create/do
</instructions>

<process>
  <step name="step_name">
    <action>Specific action to take</action>
  </step>
</process>

<best_practices>
Guidelines for optimal results
</best_practices>

<anti_patterns_to_avoid>
Common mistakes to prevent
</anti_patterns_to_avoid>

<output_instructions>
Formatting and delivery requirements
</output_instructions>
```

### Naming Conventions

- **Filename format**: `lowercase-with-hyphens.md`
- **Be descriptive**: `prd.md`, `tech-spec.md`, `user-story.md`
- **Match content**: Filename should clearly indicate the prompt's purpose

### Validation Checklist

When reviewing or editing prompts, ensure:

- [ ] XML tags are properly closed and nested
- [ ] Role definition is specific and includes expertise level
- [ ] Context provides sufficient background
- [ ] Instructions are clear and actionable
- [ ] Process steps are logical and sequential
- [ ] Output instructions specify format requirements
- [ ] Examples are included where helpful
- [ ] No duplicate or conflicting instructions

### Common XML Tags Reference

Primary structure tags:
- `<role>` - AI's identity and expertise
- `<context>` - Background and situational information
- `<instructions>` - Main directives
- `<process>` - Step-by-step workflow
- `<output_instructions>` - Formatting requirements

Supporting tags:
- `<best_practices>` - Guidelines for quality
- `<anti_patterns_to_avoid>` - Common mistakes
- `<examples>` - Sample inputs/outputs
- `<format_variations>` - Alternative approaches
- `<reminder>` - Key points to remember

Process tags:
- `<step>` - Individual process step
- `<action>` - Specific action within a step
- `<component>` - Part of a larger section
- `<tips>` - Helpful suggestions

### Testing and Quality

When adding or modifying prompts:

1. **Structure validation**: Ensure all XML tags are properly formatted
2. **Clarity check**: Instructions should be unambiguous
3. **Completeness**: All necessary sections are included
4. **Consistency**: Follows repository patterns
5. **Purpose alignment**: Prompt achieves its stated goal

### Anti-Patterns to Avoid

- Don't use inconsistent XML tag names
- Don't create overly generic prompts
- Don't omit role or context sections
- Don't use unclear or ambiguous instructions
- Don't forget to update README.md when adding new prompts
- Don't mix different formatting styles within a prompt

### File Operations

When working with prompt files:
- Always read existing prompts before creating similar ones
- Preserve XML structure when editing
- Update the README.md prompt catalog when adding new prompts
- Ensure consistent indentation (2 spaces for XML content)

## Commit Standards

Follow the Conventional Commits format: https://www.conventionalcommits.org/en/v1.0.0/
