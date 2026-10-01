
## 🗺️ The Learning Map: 5 Core Orchestration Patterns

Instead of relying on a single AI model to do everything, this framework allows you to assign specialized tasks to multiple agents. The module teaches five foundational patterns to manage how they collaborate:  

| Pattern | How It Works | Best Used For... |
|---|---|---|
| 1. Concurrent | Broadcasts the primary task to all agents at the same time and aggregates their individual findings. | Parallel analysis, independent research, or ensemble voting. |
| 2. Sequential | Passes the output of one agent as the direct input to the next agent in a rigid pipeline. | Linear, step-by-step workflows (e.g., Writer → Editor → Formatter). |
| 3. Group Chat | Agents participate in a shared, multi-turn conversation workspace moderated by a manager. | Brainstorming, maker-checker loops, and collaborative debate. |
| 4. Handoff | Control dynamically passes from one agent to another based on rules, context, or escalation paths. | Customer service routing (e.g., General Agent → Refund Specialist). |
| 5. Magentic | An AI manager dynamically updates a ledger to assign and adapt tasks to specialists on the fly. | Highly complex, open-ended tool execution and dynamic planning. |

------------------------------
## 🎯 Key Mechanics of Multi-Agent Control
When agents communicate dynamically (especially in Group Chat), they need boundaries so they don't loop forever or interrupt each other. You will learn how to configure two core strategies:  

   1. Selection Strategies: Controls who speaks next. You can use simple options like SequentialSelectionStrategy (fixed order) or smart options like KernelFunctionSelectionStrategy (an LLM judges the context to pick the next best expert). 
   2. Termination Strategies: Controls when to stop the conversation. For instance, an ApprovalTerminationStrategy can halt execution the moment a supervisor agent outputs the keyword "Approved". 

------------------------------

