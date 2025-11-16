Create a new Claude Code slash command prompt based on the user's description.

**Process:**

1. **Understand the Intent**: Ask clarifying questions about:
   - What task should this command perform?
   - What inputs does it need?
   - What output format is expected?
   - Are there any specific tools or patterns it should use?

2. **Design the Prompt**: Create a clear, actionable prompt that:
   - States the objective clearly
   - Provides step-by-step instructions
   - Includes examples where helpful
   - Specifies output format
   - Mentions relevant tools (TodoWrite, Read, Bash, etc.)

3. **Save the Command**: 
   - Suggest a command name (lowercase, hyphenated)
   - Create the `.md` file in `~/.claude/commands/`
   - Show the user the final prompt content

4. **Provide Usage Example**: Show how to use the new command

**Best Practices:**
- Keep prompts focused and single-purpose
- Use clear, imperative language
- Include context about when to use the command
- Specify expected tools or workflows
- Add examples for complex commands
