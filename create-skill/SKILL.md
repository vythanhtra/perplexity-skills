---
name: create-skill
description: Create a new Agent Skill with proper SKILL.md format and frontmatter. Use when the user wants to create a reusable skill package or edit based off an existing one.
author: Perplexity
version: '1.0'
---

# Create Skill

This skill helps you create new Agent Skills that follow the agentskills.io specification.

## When to Use This Skill

Use this skill when the user asks you to:

- Create a new skill or capability
- Package instructions into a reusable format
- Set up a skill directory

## Agent Skills Format

An Agent Skill is a directory containing a SKILL.md file with YAML frontmatter:

```
my-skill/
  SKILL.md
```

## SKILL.md Structure

**CRITICAL: When you write SKILL.md, the very first characters in the file must be `---` (the YAML frontmatter opening delimiter). Do not write any title, description, or other content before the `---`.**

```
---
name: my-skill
description: A clear description of what this skill does and when to use it.
license: (optional)
compatibility: Any environment requirements (optional)
metadata: (optional)
author: your-name
version: '1.0'
---

# Skill Title

## When to Use This Skill

Describe the scenarios where this skill should be applied.

## Instructions

Step-by-step instructions for the agent to follow.

## Examples

Include examples of inputs and expected outputs.
```

**Common mistake**: The first line of SKILL.md must be `---` (the frontmatter opening delimiter). Do NOT put any title, comment, or blank lines before it.

## Frontmatter Requirements

**Required fields:**

- `name`: 1-64 characters, lowercase alphanumeric and hyphens only
  - Must match the directory name exactly
  - Cannot start or end with hyphens
  - No consecutive hyphens allowed
  - Valid examples: `pdf-processing`, `code-review`, `data-analysis`
  - Invalid examples: `-my-skill`, `my--skill`, `My_Skill`
- `description`: 1-1024 characters describing:
  - What the skill does
  - When it should be used (important for agent discovery)
  - Should include specific keywords and trigger phrases

**Optional fields:**

- `license`: Licensing terms (e.g., MIT, Apache-2.0)
- `compatibility`: Environment requirements, max 500 characters
- `metadata`: Key-value pairs for additional information
- `allowed-tools`: Space-delimited list of pre-approved tools (experimental)

## Instructions for Creating a New Skill

1. **Understand the requirement**: Ask the user what the skill should accomplish and when it should be used.
2. **Choose a name**: Pick a descriptive, lowercase name with hyphens for word separation.
3. **Write a clear description**: This is crucial for skill discovery.
4. **Create comprehensive instructions**: Write clear, step-by-step guidance.
5. **Create the skill directory and file**: `{skills_dir}/{skill-name}/SKILL.md`
6. **Validate the skill**: `pip install -q skills-ref && agentskills validate {skills_dir}/{skill-name}`
7. **Prepare for sharing**: Single-file skill: share SKILL.md directly. Multi-file: create a `.zip` archive.
8. **Inform the user**: Let the user know the skill has been created and validated successfully.

## Common Errors

**Error: "SKILL.md must start with YAML frontmatter (---)"**
- File doesn't start with `---` on line 1
- Wrong: Starting with title `# My Skill` before `---`
- Correct: File starts immediately with `---`

**Error: Invalid name format**
- Must be 1-64 characters
- Lowercase letters, numbers, and hyphens only
- Cannot start or end with hyphen
- No consecutive hyphens (`--`)
