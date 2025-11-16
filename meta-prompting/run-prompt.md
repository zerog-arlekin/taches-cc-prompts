# run-prompt Command Documentation

The `run-prompt` command delegates prompts from `./prompts/` as sub-tasks with fresh context.

## Supported Inputs

**Single prompt execution:**
- No arguments: runs most recently created prompt
- Prompt number (e.g., "001", "5")
- Partial filename (e.g., "user-auth")

**Multiple prompts:**
- Multiple numbers with optional execution flag
- Defaults to sequential execution for safety when no flag specified

## Execution Strategies

The command supports three modes:

1. **Single prompt**: Reads file, delegates via Task tool, archives to completed folder
2. **Parallel execution**: "Spawn all Task tools in a SINGLE MESSAGE" for simultaneous processing
3. **Sequential execution**: Processes prompts one at a time, waiting for completion before starting next

## Key Requirements

- File matching uses zero-padded numbers ("5" finds "005-_.md")
- Multiple matches prompt user selection
- Parallel calls must be in one message (critical for functioning)
- Sequential mode halts on failure
- Archive prompts only after successful completion
