# User Prompt Examples for AutoGen Studio Agents

This document contains example user prompts that demonstrate how to effectively engage with different types of AutoGen Studio agent systems. These examples show the level of detail and context needed to get the best results from your AI agents.

---

## Example 1: Enterprise Infrastructure & Analytics

### User Prompt: Transport for Fictitious State Data Platform

**Context**: Chief Data Officer at Transport for Fictitious State

**Prompt**:
```
I am the Chief Data Officer at Transport for NSW. Lately we have been having different service interruptions and issues causing minor and major delays in the network. For example, recently the high-voltage live wire got entangled with the train and caused incredibly major delays across the whole network, which also slowed things down with our buses and our light rail and our Sydney Metro.

I want to come up with a modern analytics platform so that in the event a future disruption happens, I want to find out how I can leverage my existing data to reroute buses and light rail and Sydney Metro to accommodate and replace services. Our normal process is that when a distruption like this happens to our network, we also reach out to Uber to negotiate a capped surcharge so everyone is able to get to work or home safely in a cost effective manner.

As you know, we have services and data sources at our AWS cloud, Snowflake, and in our Azure cloud. So please keep that in the back of your mind. I also want to leverage by existing PowerBI and Microsoft Fabric, but some of our teams also uses Azure Databricks.
```

**Why This Works**:
- **Clear Role Definition**: Establishes authority and context (Chief Data Officer)
- **Specific Problem**: Real-world scenario with concrete impact
- **Business Context**: Explains the operational challenge and consequences
- **Technical Constraints**: Mentions existing multi-cloud infrastructure
- **Solution Direction**: Indicates preference for Microsoft Fabric while acknowledging existing tools
- **Scope Clarity**: Focuses on predictive rerouting capabilities

**Best For**: Microsoft Data & AI Agents (GBB, Pre-sales, STU, Customer Reviewer)

---

## Example 2: Personal/Professional Content Creation

### User Prompt: Microsoft Blog Post Writing Assistant

**Context**: Professional seeking writing assistance for technical blog content

**Prompt**:
```
I want to provide my comprehensive writing and then using the agentic framework and details below, help me create the right number of agents to review my writing before I post on a Microsoft blog? Include an editor, a fact checker, and someone who represents my target audience who is someone in the technology industry but leans more towards business outcomes and impact rather than technical details.
```

**Why This Works**:
- **Clear Objective**: Wants writing review and optimization
- **Specific Platform**: Microsoft blog (implies style and audience expectations)
- **Agent Requirements**: Requests specific types of reviewers
- **Audience Definition**: Clear target audience description (tech industry, business-focused)
- **Quality Standards**: Implies high standards needed for Microsoft publication

**Best For**: Writing Assistant Agents (Orchestrator, Content Editor, Technical Reviewer, Audience Optimizer, Grammar & Style Specialist)

---

## Key Elements of Effective Prompts

### 1. **Role & Context**
- Who you are and your authority/perspective
- Organizational context and constraints
- Industry or domain specifics

### 2. **Problem Definition**
- Specific challenge or goal
- Real-world examples and impacts
- Current state vs. desired state

### 3. **Technical Environment**
- Existing systems and tools
- Preferences and constraints
- Integration requirements

### 4. **Success Criteria**
- What good looks like
- Specific outcomes needed
- Quality or performance expectations

### 5. **Audience Considerations**
- Who will use or consume the output
- Level of technical detail required
- Business vs. technical focus

---

## Prompt Structure Template

```
**Context**: [Your role and organization]

**Challenge**: [Specific problem or goal]

**Current State**: [Existing systems, tools, constraints]

**Desired Outcome**: [What success looks like]

**Additional Requirements**: [Special considerations, preferences, constraints]

**Content/Data**: [Attach or include relevant materials]
```

---

## Tips for Better Agent Interactions

### ✅ **Do This**:
- Provide real-world context and examples
- Be specific about your role and authority
- Mention existing tools and constraints
- Define your target audience clearly
- Include success criteria and quality expectations

### ❌ **Avoid This**:
- Vague or generic requests
- Assuming agents know your context
- Leaving out important constraints
- Not specifying the intended audience
- Being unclear about desired outcomes

---

## Advanced Prompt Techniques

### **Multi-Stage Prompting**
For complex projects, break your request into phases:
1. **Discovery**: "Help me understand the problem space"
2. **Planning**: "Create a solution architecture"
3. **Implementation**: "Provide detailed implementation steps"
4. **Review**: "Validate and optimize the approach"

### **Constraint-Based Prompting**
Explicitly state your limitations:
- Budget constraints
- Timeline requirements
- Technical limitations
- Regulatory compliance needs
- Existing vendor relationships

### **Outcome-Focused Prompting**
Frame requests around business outcomes:
- "Reduce operational costs by X%"
- "Improve customer satisfaction scores"
- "Increase system reliability to 99.9%"
- "Enable real-time decision making"

---

## Example Variations

### **For Technical Deep-Dives**:
"I need detailed technical architecture recommendations for [specific scenario] that integrates with [existing systems] and meets [specific requirements]."

### **For Business Case Development**:
"Help me build a compelling business case for [solution] that addresses [business challenges] and demonstrates ROI to [stakeholder audience]."

### **For Content Creation**:
"Review and optimize my [content type] for [target audience] to achieve [specific goals] while maintaining [quality standards]."

### **For Strategic Planning**:
"Develop a strategic roadmap for [initiative] that considers [current state], [constraints], and [future vision]."
