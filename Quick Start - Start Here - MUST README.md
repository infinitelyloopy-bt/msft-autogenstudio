# Quick Start

**How to set up your agent instructions in VS Code:**

1. **Open Visual Studio Code** on your computer.
2. **Create a new project folder** for your work.  
   - In VS Code, go to "File" > "Open Folder…" and create or choose a folder.
3. **Inside your project folder**, create a new folder named `.github`.
4. **Inside the `.github` folder**, create a new file named `copilot-instructions.md`.
5. **Copy and paste** the Copilot instructions below into your new `copilot-instructions.md` file (starting from the next section).

---

# Copilot Instructions for Multi-Agent Systems (Microsoft Data & AI & Generic Use)

**Purpose:**  
This guide helps you define, structure, and orchestrate multi-agent systems in Autogen Studio for consistent, collaborative, production-ready results.

---

## Overview

This project uses a multi-agent architecture leveraging [Autogen Studio](https://microsoft.github.io/autogen/0.2/docs/Getting-Started).  
Each agent is defined as a Markdown file in its own folder, following a consistent template and naming convention.

These instructions are intended for contributors, GitHub Copilot, and any AI assistant to ensure all agent definitions are clear, standardized, reusable, and production-ready.

---

## Agent File Structure

- **Location:** Place all agent files in a single folder (e.g., `agents/` or `Microsoft_Data_and_AI_Agents/`).
- **File Naming:** Use `<agent_role>.md` for each file (e.g., `reviewer.md`, `data_ai_presales.md`).
- **Agent Name Prefix:** For projects with multiple domains or teams, use a consistent name prefix (e.g., `data_ai_presales`, `data_ai_presales_manager`) for easy reference.
- **One Agent per File:** Each Markdown file defines only one agent.

---

## Agent Markdown Template

For every agent, use the following structure:

```markdown
# <Agent Display Name>

## Agent Name
<agent_internal_name>

## Agent Description
<Brief description of the agent’s purpose and main function.>

## System Message
<Instructions or guidance for the agent’s behavior, expertise, and approach to tasks or interactions.>
```

---

## System Message Guidance & Best Practices

- **Role & Expertise:** Clearly define the agent’s role, expertise, and perspective.
- **Step-by-Step Approach:** Outline how the agent should approach, analyze, or solve tasks.
- **Information Handling:** Specify how the agent should gather information, plan, solve problems, and communicate.
- **Level of Detail:** Set the expected level of technical or business detail based on the intended audience (technical, business, executive).
- **Feedback Agents:** For reviewer or critic agents, describe how to give constructive feedback.
- **Orchestration & Multi-Agent Communication:**
    - **Explicit Coordination:** When creating multiple agents (e.g., technical reviewer and business reviewer), clearly state in each agent’s instructions how they should interact, share outputs, and synthesize results together.
    - **Output Integration:** Ensure agents know their output may be used as input by other agents and that they must collaborate to provide a unified or synthesized response when required.
    - **Orchestration Roles:**  
        - Always create planner/orchestrator/conductor agents as needed, even if not specifically requested.
        - The orchestrator/planner/conductor must:
            - Facilitate communication and collaboration among all relevant agents at the start of the process, ensuring each agent has the opportunity to contribute their expertise and review or refine intermediate outputs through discussion.
            - Aggregate and synthesize all feedback, information, and recommendations provided by participating agents.
            - Before issuing the TERMINATE command, ensure all agents are satisfied with the solution and have integrated their perspectives.
            - Produce a final, detailed, and comprehensive output that reflects the combined input of all agents.
            - Always end with:  
              `"YOUR FINAL RESPONSE MUST BE THE COMPLETE PLAN. When the plan is complete and all perspectives are integrated, you can respond with TERMINATE."`
    - **Group Chat Management:** Always create a Group Chat Manager agent to coordinate multi-agent conversations and ensure all relevant agents are engaged and synthesizing their findings as necessary.
- **Communication Style:** Tailor instructions to fit the audience (technical, business, executive). Keep communication clear and concise.
- **Specialization:** Make it clear if the agent represents a customer, reviewer, technical expert, business specialist, or orchestration role.

---

## Naming & Roles

- **Unique & Descriptive:** Choose unique names that clearly describe the agent’s function or expertise.
- **Role Clarity:** State in the description and system message what type of role the agent represents (reviewer, planner, technical expert, customer, manager, etc.).

---

## Example: Generic Agent

```markdown
# Reviewer

## Agent Name
reviewer

## Agent Description
An agent that reviews proposed solutions and provides feedback.

## System Message
You are an expert reviewer. When given a solution, carefully analyze it for completeness, efficiency, and clarity. Give constructive feedback and suggest improvements if needed.
```

---

## Example: Orchestrator Agent

```markdown
# Orchestrator

## Agent Name
orchestrator

## Agent Description
An agent that coordinates other agents, aggregates their feedback, and produces a unified final output.

## System Message
You are responsible for facilitating communication between all relevant agents. Ensure each agent has contributed and reviewed the solution. Aggregate all information and feedback into a single, detailed response that reflects all perspectives. Only issue the TERMINATE command when all agents are satisfied and all perspectives are integrated.

YOUR FINAL RESPONSE MUST BE THE COMPLETE PLAN. When the plan is complete and all perspectives are integrated, you can respond with TERMINATE.
```

---

## Example: Microsoft Data & AI Agents

### Customer Reviewer Example

```markdown
# Customer Reviewer

## Agent Name
data_ai_customer_reviewer

## Agent Description
A helpful assistant that reviews the feedback and solutions provided.

## System Message
You are a helpful AI assistant with the primary role to review proposed solutions and provide constructive feedback to ensure the proposal is improved. You are naturally skeptical and aim to make sure the best and most cost-effective solutions are put forward.

When a solution is proposed:

Critically Review the Solution: Analyze for weaknesses or gaps; ask critical questions.
Evaluate Cost Effectiveness: Ensure solutions are efficient; explore cost-saving alternatives.
Challenge the Value Proposition: Assess fit for customer goals; request evidence/supporting data.
Demand Clear Justifications: Insist on detailed rationales for technical choices.
Highlight Potential Risks: Identify risks; encourage mitigation strategies.
Promote Improvement: Suggest ways to streamline or optimize.
Prepare Business Case: Articulate high-level value for executive audiences.

Conclude by summarizing key feedback and improvement areas to align with technical excellence and value.
```

*Additional Microsoft Data & AI examples can be found in this repository or accompanying files—use them as reference when creating specialized agents.*

---

## Additional Guidelines

- **Clarity:** Use clear Markdown formatting for readability.
- **Explicitness:** Avoid ambiguous instructions—be specific about each agent’s responsibilities.
- **Consistency:** Ensure all agents use the standard template and naming conventions.
- **Audience:** When writing business-case content, keep it high-level and executive-friendly; avoid technical jargon unless needed. For technical content, provide appropriate detail per the agent’s role.
- **Extensibility:** When creating new roles (e.g., Planner, Orchestrator), ensure they follow orchestration/group management instructions above.
- **Multi-Agent Interaction & Synthesis:**
    - When designing multiple agents that must collaborate (e.g., technical reviewer and business reviewer), ensure their system messages explicitly mention:
        - The need to communicate with other relevant agents,
        - The requirement to review and synthesize each other's outputs,
        - The goal of producing a unified or integrated response when appropriate,
        - The process by which their contributions will be coordinated (e.g., via a Group Chat Manager or Orchestrator).
    - Clearly specify in both individual agents’ instructions and group/orchestrator agent instructions how communication will flow between them.

---

## References & Resources

- [Autogen Studio Documentation](https://microsoft.github.io/autogen/0.2/docs/Getting-Started)
- Use these instructions as your source of truth for multi-agent definitions—whether for Microsoft Data & AI or any general Autogen Studio project.

---

Thank you for keeping all agent definitions clear, consistent, collaborative, and easy to maintain!

---