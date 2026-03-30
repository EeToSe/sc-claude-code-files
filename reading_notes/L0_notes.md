# Course Introduction

Welcome to "Claude Code: A highly Agentic Coding Assistant"! Before you get started with the course, you are encouraged to read this note so you can get an idea about the course outline and how to best navigate this course. 

## Course Note

### AI-assisted coding evolution

Occasional Q&A with LLMs  
→ IDE autocomplete (e.g., GitHub Copilot)  
→ Semi-autonomous coding tools  
→ Highly agentic assistants (Claude Code can execute multi-step tasks for many minutes)  
→ Multi-agent orchestration (developers run several Claude instances in parallel across different parts of a codebase)

A key tip for working with Claude Code is to **provide clear context so it can complete your task efficiently**. In practice, this means:

- Pointing Claude Code to the relevant files
- Clearly describing the features and functionality you want
- Extending its capabilities with MCP servers and other tools in the ecosystem

### Simple underlying architecture
Claude Code’s architecture can be understood in three layers:

1. **A different way of understanding code**  
   Instead of first building semantic embeddings and then retrieving results, Claude Code works more like an engineer: it actively reads files, follows references, searches patterns, lists directories, and uses tools like regex to trace how the codebase fits together.

2. **A different way of working**  
   Instead of answering one isolated question at a time, Claude Code can stay on a single objective and **execute it across multiple steps, continuously advancing the task over time**.

3. **A different way of organizing memory**  
   Instead of relying only on chat context, Claude Code can externalize findings into notes (for example, in `Claude.md`), preserving discoveries and using them to make better decisions as work progresses.

## Course Activities - Cost Visibility

If you'd like to install Claude Code to try the lessons:
- you can have a Pro (`$20`/month) or Max (`$100`/month) [subscription](https://www.anthropic.com/claude-code#:~:text=Pro,Sign%20up). The pro subscription is enough for the lessons' activities, but **it doesn't include Opus**. 
- Or, you can be billed based on **API usage** (if you just use sonnet for all the lessons' activities, the total cost for all lessons can be between `$12` and `$20`). In a given session, you can monitor the cost using the `/cost` command.


## Course Prerequisites

You can take the course whether you're a developer, a data scientist/analyst or even non-technical. But to make the best out of the course and to understand the details of the prompts used:
- Basic familiarity of Python is required for lessons 2-7. 
- For lesson 8, the app you'll build is a Next.js app so you may need to be familiar with this framework if you'd like to check the code generated, but don't worry if you're not, you can still try the last lesson to learn how you can use Figma MCP server to import the mock design into Claude's context. 
- Understanding of basic terminal commands would be also helpful. 
- Familiarity with basic git commands would be great (`git add, commit, pull, push`).
