# Autogen Studio Agents for Microsoft DEMO

> This repository provides a comprehensive library of multi-agent systems and reusable agent definitions for [Autogen Studio](https://microsoft.github.io/autogen/0.2/docs/Getting-Started), with a focus on Microsoft Data & AI and writing assistance. All agents follow a standardized template and orchestration model for clarity, collaboration, and production-readiness.


## Repository Structure

- **Microsoft_Data_AI_Agents/**  
  Agents for Data & AI scenarios, including presales, specialist, planner, customer, reviewer, researcher, group chat manager, and security reviewer roles. See `Microsoft_Data_AI_Agents/README.md` for details.

- **Writing_Assistant_Agents/**  
  A set of 5 specialized agents for reviewing and optimizing written content (blog posts, articles, papers):
  - Orchestrator: Coordinates the review process and synthesizes all feedback.
  - Content Editor: Improves structure, flow, and clarity.
  - Grammar & Style Specialist: Ensures language is correct and consistent.
  - Technical Reviewer: Checks for accuracy and credibility.
  - Audience Optimizer: Ensures content is relevant and engaging for the target audience.
  See `Writing_Assistant_Agents/README.md` for an overview.

- **Examples/**  
  Example user prompts and usage scenarios. See `Examples/User Prompts.md` for up-to-date prompt examples for all agent systems.

- **.github/copilot-instructions.md**  
  The authoritative guide for contributors and AI assistants, detailing agent design standards, templates, naming conventions, and orchestration best practices. **All agent definitions must follow the Markdown template and orchestration guidance in this file.**
## Agent Design & Standards

All agents are defined in Markdown files using a consistent template and naming convention, as described in `.github/copilot-instructions.md`. This ensures:

- Clarity and reusability of agent definitions
- Explicit orchestration and multi-agent collaboration
- Easy extension and maintenance

**Key points:**

- Each agent is defined in its own Markdown file and grouped by domain or function in dedicated folders.
- Orchestrator, planner, and group chat manager agents are included for multi-agent coordination.
- System messages for each agent specify their role, expertise, and collaboration requirements.
- **All new agents must follow the Markdown template and orchestration rules in `.github/copilot-instructions.md`.**
## Usage

1. Review agent definitions in the relevant folder for your scenario (Data & AI, Writing Assistance).
2. Use the provided templates and orchestration patterns to build your own multi-agent workflows in Autogen Studio.
3. Reference `Examples/User Prompts.md` for sample prompts and usage patterns for all agent systems.
4. Follow the standards in `.github/copilot-instructions.md` for any new agent or system contributions.

## References & Resources

- [Autogen Studio Documentation](https://microsoft.github.io/autogen/0.2/docs/Getting-Started)
- [copilot-instructions.md](.github/copilot-instructions.md)
- [Microsoft_Data_AI_Agents/README.md](Microsoft_Data_AI_Agents/README.md)
- [Writing_Assistant_Agents/README.md](Writing_Assistant_Agents/README.md)

For questions or contributions, see the guidelines in `.github/copilot-instructions.md`.
# Welcome to the AutoGen Studio Workshop! 🚀

**Empowering Everyone at Microsoft Asia to Explore AI – No Coding Required!**

This workshop is designed for non-technical team members who want to confidently use AI tools like AutoGen Studio. You don't need a coding background or technical expertise – just curiosity and a willingness to learn!

## 🌟 Workshop Overview

**What**: Hands-on introduction to AutoGen Studio (v0.1.5)  
**Who**: Non-technical Super Heroes  
**How**: Interactive Teams sessions (check your invites for details)  
**Why**: To build confidence, learn to follow technical instructions, and discover new ways to work smarter with AI for personal and professional development

## 📝 What You'll Learn

- How to set up and use AutoGen Studio (v0.1.5) on your own computer
- How to use GitHub for collaboration (even if you've never coded!)
- How to find answers and keep learning using free resources like YouTube and Copilot

## 🛠️ Prerequisites

### 1. Install Visual Studio Code

AutoGen Studio works best with a good code editor for managing your agent files and configurations.

- Go to [code.visualstudio.com](https://code.visualstudio.com/)
- Download the latest version for your operating system (Windows, Mac, or Linux)
- Install with default settings
- Launch VS Code to verify installation

💡 **Why VS Code?** It provides excellent support for managing AutoGen Studio agent files, has built-in GitHub integration, and works seamlessly with GitHub Copilot for enhanced productivity.

### 2. Install Python (Windows & Mac)

AutoGen Studio requires Python (version 3.8–3.12). Installing version 3.12 is ideal.

- Go to [python.org/downloads](https://python.org/downloads)
- Download and install a compatible version (check "Add Python to PATH" during setup for Windows)
- To verify installation:
  
  **Windows users:**
  1. Press `Windows key + R`, type `cmd`, and press Enter to open Command Prompt
  2. Type `python --version` and press Enter
  
  **Mac users:**
  1. Press `Cmd + Space`, type `terminal`, and press Enter to open Terminal
  2. Type `python3 --version` and press Enter

- You should see a version between 3.8 and 3.12.

⚠️ **Important**: AutoGen Studio v0.1.5 does not support Python 3.13 or newer.  
📖 See [Getting Started Guide](https://microsoft.github.io/autogen/0.2/docs/Getting-Started).

### 3. Install pip

Check if pip is installed:

**Windows users:**
1. Open Command Prompt (press `Windows key + R`, type `cmd`, press Enter)
2. Type `pip --version` and press Enter

**Mac users:**
1. Open Terminal (press `Cmd + Space`, type `terminal`, press Enter)
2. Type `pip3 --version` and press Enter

If it's not found, follow the [pip installation guide](https://pip.pypa.io/en/stable/installation/).

### 4. Install AutoGen Studio

Once Python and pip are ready:

**Windows users:**
1. Open Command Prompt (press `Windows key + R`, type `cmd`, press Enter)
2. Type `pip install autogenstudio==0.1.5` and press Enter

**Mac users:**
1. Open Terminal (press `Cmd + Space`, type `terminal`, press Enter)
2. Type `pip3 install autogenstudio==0.1.5` and press Enter

📚 More details here: [AutoGen Studio Docs](https://microsoft.github.io/autogen/0.2/docs/Getting-Started)

### 5. Install OpenAI Python Library

Once you have installed AutoGen Studio:

**Windows users:**
1. In the same Command Prompt window, type `pip install openai` and press Enter

**Mac users:**
1. In the same Terminal window, type `pip3 install openai` and press Enter

## 🧰 GitHub Essentials & Copilot Setup

### 1. Create a GitHub Account

If you don't already have one: [github.com/join](https://github.com/join)  
You will need to create a personal account that you will link to your name@microsoft.com account

### 2. Activate Your GitHub Copilot Benefits

- Visit [aka.ms/copilot](https://aka.ms/copilot)
- Sign in with your GitHub account
- Follow the instructions to activate your employee Copilot benefit

## 📁 How to Use This GitHub Repo

1. **Sign In**: Use the GitHub account you created
2. **Explore Tabs**:
   - `Code` – View workshop files
   - `Issues` – Ask questions or share feedback
   - `Pull Requests` – Not needed for this workshop
3. **Create an Issue**:
   - Go to the `Issues` tab
   - Click "New Issue"
   - Add a clear title and describe your question or problem
4. **Join Discussions**:
   - Click on any issue to comment or reply

💡 **You don't need to code** — GitHub is your collaboration space!

## 📚 Keep Learning: Free Resources

- [AutoGen Studio Docs](https://microsoft.github.io/autogen/0.2/docs/Getting-Started)
- [Microsoft Copilot](https://copilot.microsoft.com/)
- [GitHub Docs: Getting Started](https://docs.github.com/en/get-started)
- [VS Code Getting Started](https://code.visualstudio.com/docs)

## 🙋‍♂️ Need Help?

Join one of the Teams sessions or post a question in the Issues tab — we're here to support you.

## 💬 Final Word

You don't have to be technical to make a difference. Let's explore the world of AI together! 🌍✨

---


## 📂 Repository Contents

This repository contains:



### 🎯 Agent Systems

- **Writing Assistant Agents** – A set of 5 specialized agents for reviewing and optimizing written content: Orchestrator, Content Editor, Grammar & Style Specialist, Technical Reviewer, Audience Optimizer.
- **Microsoft Data & AI Agents** – A comprehensive team of specialized agents representing different roles in Microsoft's Data & AI organization for customer engagements

### 📖 Documentation & Resources

- **Setup Guides** - Step-by-step instructions for getting started with AutoGen Studio
- **Architecture Diagrams** - Visual workflows and team interaction patterns for both agent systems
- **Examples** - Practical demonstrations and user prompt examples for both agent systems
- **Quick References** - Fast-access guides for daily use and agent capabilities
- **Usage Examples** - Detailed scenarios showing how to effectively use each agent system

### 🚀 What You Can Do

- **Content Creation**: Transform drafts into polished, professional content
- **Customer Engagements**: Simulate realistic Microsoft Data & AI team interactions
- **Business Solutions**: Get expert perspectives on data, AI, security, and business strategy
- **Learning & Practice**: Build confidence with AI tools in a safe, structured environment

Explore the folders above to discover powerful AI agents that can help with both content optimization and Microsoft customer engagement scenarios!
