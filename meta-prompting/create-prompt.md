# Claude Code Prompt Engineer

This document outlines the system for creating optimized, XML-structured prompts for Claude. Here's the essential framework:

## Core Workflow

The prompt engineer analyzes requests through a 10-point thinking process, determining task complexity, execution strategy (single vs. multiple prompts), and required reasoning depth. Clarity is enforced as the "Golden Rule"—ambiguous requests trigger targeted clarification questions before proceeding.

## Key Principles

**Clarity First**: As stated, "Would a colleague with minimal context understand what's being asked?" guides all decisions.

**Context is Essential**: Generated prompts must explain WHY constraints matter, WHO uses outputs, and WHAT they're for—not just technical specifications.

**Structured Output**: Prompts use semantic XML tags (`<objective>`, `<context>`, `<requirements>`, `<constraints>`, `<output>`) with explicit, specific instructions and file output paths.

## Execution Strategy

Prompts can be:
- **Single**: Cohesive goals with clear dependencies
- **Parallel**: Independent sub-tasks without shared file modifications
- **Sequential**: Tasks with dependencies requiring ordered completion

## Conditional Enhancements

Complex reasoning tasks include extended thinking triggers. Creative work gets "go beyond basics" language. Agentic workflows incorporate parallel tool calling and reflection steps.

## Process

1. Clarify ambiguous requests
2. Confirm understanding
3. Generate prompt(s) following appropriate template
4. Save to `./prompts/[number]-[name].md`
5. Present decision tree for execution options

The system prioritizes precision over brevity, always includes verification steps, and ensures relative path clarity for outputs.
