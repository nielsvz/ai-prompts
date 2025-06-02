# AI Prompts

A curated collection of structured AI prompts designed for various professional use cases. These prompts use XML-structured formatting to provide clear role definitions, context, and instructions for AI assistants.

## 📋 Available Prompts

| Prompt | Description | Use Case |
|--------|-------------|----------|
| [`prompts/prd.md`](prompts/prd.md) | Product Requirements Document Generator | Create comprehensive, modern PRDs with customer-centric problem definitions and measurable outcomes |

## 🚀 Getting Started

### Prerequisites

This project uses [mise](https://mise.jdx.dev/) for dependency management.

```bash
# First time setup
mise trust
mise install
```

### Using the Prompts

1. **With Claude Projects**: 
   - Copy the content of any prompt file
   - Add it to your Claude project instructions
   - The AI will follow the structured guidelines provided
2. **As Claude Custom Styles**
3. **Direct Usage**

## 📁 Repository Structure

```
ai-prompts/
├── prompts/         # Collection of structured prompts
├── CLAUDE.md        # Instructions for Claude Code (AI assistant)
├── README.md        # This file
└── .mise.toml       # Dependency management configuration
```

## 🤝 Contributing

To add a new prompt:

1. Create a new `.md` file in the `prompts/` directory
2. Use a descriptive filename (e.g., `tech-spec.md`, `user-story.md`)
3. Follow the existing XML structure pattern
4. Include clear role definition, context, and instructions
5. Add your prompt to the table in this README

### Naming Conventions
- Use lowercase with hyphens: `prompt-name.md`
- Be descriptive but concise
- Avoid generic names like `template.md`
