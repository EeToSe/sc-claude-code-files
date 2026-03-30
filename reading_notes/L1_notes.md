# What is Claude Code?

## Agentic System = Model+Tools+Environment+Control Loop
![alt text](../images/harness.png)
1. **Lightweight Harness**: Instead of talking directly to a model, Claude Code provides a lightweight harness accessed through the command line to leverage the model's intelligence for complex coding tasks.

2. **Tools & Environment**: The harness equips the model with tools, an environment, and supporting functionality to navigate codebases and solve complex problems more effectively than direct task assignment.

3. **Memory & Action**: The model gains memory to retain user preferences and task context, plus the ability to assess data needs, formulate plans, and take action.

## Use scenarios
Claude Code can help with **every step** of your project.

![use-scenarios](../images/use-scenarios.png)

## Tool use
![alt text](../images/tool-use.png)
The architectural pattern is the same as [ELEC4633
Real Time Engineering](https://www.unsw.edu.au/content/dam/pdfs/engineering/electrical-telecom-eng/course-outlines/2021-10-electrical-engineering/term-1-(and-summer-term-2021)/2021-10-ELEC4633-T1-2021-Course-Outline.pdf): a system where components communicate by passing messages and invoking actions, with a **coordinator** in the middle managing who does what.

## Claude's memory
Memory across sessions (claude.md):
- In `CLAUDE.md` files, you can define your style guidelines and common commands.
- Claude.md files get automatically loaded into Claude Code's context when launched.

Conversation history:
- Conversation history is automatically stored locally on `~/.claude/history.jsonl`.
- You can choose to clear the conversation of your current session.
- Past conversations are not automatically included in the context. You manually ask Claude Code to continue a previous conversation.

User control & extension:
- Slash Commands: Users can actively guide Claude to record or modify memory via commands like `/remember`, `/forget`, and `/summarize`.
- Memory is persisted in `CLAUDE.md` files — globally at `~/CLAUDE.md` or per-project at `./project/CLAUDE.md`. Project-level settings take priority over global ones.
- Community plugins (e.g. `claude-mem`) can further enhance local memory by auto-detecting the tech stack and storing session summaries, reducing token usage on repeated context injection.


## Claude Code Installation

To follow along with the lessons, here's how you can install Claude Code.

1. Run the following command:

    `npm install -g @anthropic-ai/claude-code`

    For more installation guides, you can find them [here](https://docs.anthropic.com/en/docs/claude-code/setup).


2. Once you have Claude Code installed, you can:
   - launch it from your terminal: navigate to your project folder & then type `claude`
   - launch it from the terminal integrated within VS Code by typing `claude`, the extension will auto-install.

    For more info, check [Claude Code IDE Integrations](https://docs.anthropic.com/en/docs/claude-code/ide-integrations).
