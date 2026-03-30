# Lesson 6: References to GitHub Integration & Hooks

## GitHub Integration

Claude Code GitHub Actions brings Claude to your GitHub workflow. Once you set it up, you can **mention `@claude` in any pull request or issue**. It can implement code, create pull request and review code. The easiest way to set it up this is through Claude Code in the terminal by running `/install-github-app`.

You can check the documentation [here](https://docs.anthropic.com/en/docs/claude-code/github-actions) for more information on how to use this integration. 

## Hooks

Claude Code hooks are shell commands that you can define and can be executed at various points in Claude Code’s lifecycle (before tool execution, after tool execution, when subagent finishes a task, when claude finishes responding).  

We showed a quick example on hooks in this lesson. If you'd like to learn more about hooks and see more examples, you are encouraged to check out:
- "Hooks" in Anthropic's [Claude Code In action](https://anthropic.skilljar.com/claude-code-in-action/312000).
- Documentation: [Hooks guide](https://docs.anthropic.com/en/docs/claude-code/hooks-guide) and [hooks reference](https://docs.anthropic.com/en/docs/claude-code/hooks).

## Summary of Claude Code Features
**GitHub Integration**:
- Claude Code GitHub Actions allows you to mention `@claude` in pull requests or issues to:
  - Review code
  - Implement code
  - Create pull requests
- Set it up easily by running `/install-github-app` in the terminal.

**Hooks**
- Claude Code hooks are shell commands integrated into the system.
- Hooks are triggered at **specific stages** in Claude Code’s lifecycle (e.g., before or after executing a tool, or when a subagent completes a task).
- Hooks solve the critical problem of how to constrain and monitor an autonomous AI agent.