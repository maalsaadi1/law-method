# Law Method Knowledge Base

## INDEX OF TOPICS

- [Law Method Knowledge Base](#Law-Method-knowledge-base)
  - [INDEX OF TOPICS](#index-of-topics)
  - [Law Method - CORE PHILOSOPHY](#Law-Method---core-philosophy)
  - [Law Method - AGILE METHODOLOGIES OVERVIEW](#Law-Method---agile-methodologies-overview)
    - [CORE PRINCIPLES OF AGILE](#core-principles-of-agile)
    - [KEY PRACTICES IN AGILE](#key-practices-in-agile)
    - [BENEFITS OF AGILE](#benefits-of-agile)
  - [Law Method - ANALOGIES WITH AGILE PRINCIPLES](#Law-Method---analogies-with-agile-principles)
  - [Law Method - TOOLING AND RESOURCE LOCATIONS](#Law-Method---tooling-and-resource-locations)
  - [Law Method - COMMUNITY AND CONTRIBUTIONS](#Law-Method---community-and-contributions)
    - [Licensing](#licensing)
  - [Law Method - ETHOS \& BEST PRACTICES](#Law-Method---ethos--best-practices)
  - [AGENT ROLES AND RESPONSIBILITIES](#agent-roles-and-responsibilities)
  - [NAVIGATING THE Law Method WORKFLOW - INITIAL GUIDANCE](#navigating-the-Law-Method-workflow---initial-guidance)
    - [STARTING YOUR PROJECT - ANALYST OR PM?](#starting-your-project---analyst-or-pm)
    - [UNDERSTANDING EPICS - SINGLE OR MULTIPLE?](#understanding-epics---single-or-multiple)
  - [GETTING STARTED WITH Law Method](#getting-started-with-Law-Method)
    - [Initial Project Setup](#initial-project-setup)
    - [Exporting Artifacts from AI Platforms](#exporting-artifacts-from-ai-platforms)
    - [Document Sharding](#document-sharding)
    - [Utilizing Dedicated IDE Agents (Task Manager, Researcher, GitHub Expert, and Dev)](#utilizing-dedicated-ide-agents-task-manager-researcher-github-expert-and-dev)
    - [When to Use the Law Method IDE composer](#when-to-use-the-Law-Method-ide-composer)
  - [SUGGESTED ORDER OF AGENT ENGAGEMENT (TYPICAL FLOW)](#suggested-order-of-agent-engagement-typical-flow)
  - [HANDLING MAJOR CHANGES](#handling-major-changes)
  - [IDE VS UI USAGE - GENERAL RECOMMENDATIONS](#ide-vs-ui-usage---general-recommendations)
    - [CONCEPTUAL AND PLANNING PHASES](#conceptual-and-planning-phases)
    - [TECHNICAL DESIGN, DOCUMENTATION MANAGEMENT \& IMPLEMENTATION PHASES](#technical-design-documentation-management--implementation-phases)
    - [Law Method FILES](#Law-Method-files)
  - [LEVERAGING IDE TASKS FOR EFFICIENCY](#leveraging-ide-tasks-for-efficiency)
    - [PURPOSE OF IDE TASKS](#purpose-of-ide-tasks)
    - [EXAMPLES OF TASK FUNCTIONALITY](#examples-of-task-functionality)

## Law Method - CORE PHILOSOPHY

**STATEMENT:** "Vibe CEO'ing" is about embracing the chaos, thinking like a CEO with unlimited resources and a singular vision, and leveraging AI as your high-powered team to achieve ambitious goals rapidly. The Law Method (Law Method), with the integrated "Law Method Orchestrator Agent", elevates "vibe coding" to advanced project planning, providing a structured yet flexible framework to plan, execute, and manage software projects using a team of specialized AI agents.

**DETAILS:**

- Focus on ambitious goals and rapid iteration.
- Utilize AI as a force multiplier.
- Adapt and overcome obstacles with a proactive mindset.

## Law Method - AGILE METHODOLOGIES OVERVIEW

### CORE PRINCIPLES OF AGILE

- Individuals and interactions over processes and tools.
- Working software over comprehensive documentation.
- Customer collaboration over contract negotiation.
- Responding to change over following a plan.

### KEY PRACTICES IN AGILE

- Iterative Development: Building in short cycles (sprints).
- Incremental Delivery: Releasing functional pieces of the product.
- Daily Stand-ups: Short team meetings for synchronization.
- Retrospectives: Regular reviews to improve processes.
- Continuous Feedback: Ongoing input from stakeholders.

### BENEFITS OF AGILE

- Increased Flexibility: Ability to adapt to changing requirements.
- Faster Time to Market: Quicker delivery of valuable features.
- Improved Quality: Continuous testing and feedback loops.
- Enhanced Stakeholder Engagement: Close collaboration with users/clients.
- Higher Team Morale: Empowered and self-organizing teams.

## Law Method - ANALOGIES WITH AGILE PRINCIPLES

The Law Method, while distinct in its "Vibe CEO'ing" approach with AI, shares foundational parallels with Agile methodologies:

- **Individuals and Interactions over Processes and Tools (Agile) vs. Vibe CEO & AI Team (Law Method):**

  - **Agile:** Emphasizes the importance of skilled individuals and effective communication.
  - **Law Method:** The "Vibe CEO" (you) actively directs and interacts with AI agents, treating them as a high-powered team. The quality of this interaction and clear instruction ("CLEAR_INSTRUCTIONS", "KNOW_YOUR_AGENTS") is paramount, echoing Agile's focus on human elements.

- **Working Software over Comprehensive Documentation (Agile) vs. Rapid Iteration & Quality Outputs (Law Method):**

  - **Agile:** Prioritizes delivering functional software quickly.
  - **Law Method:** Stresses "START_SMALL_SCALE_FAST" and "ITERATIVE_REFINEMENT." While "DOCUMENTATION_IS_KEY" for good inputs (briefs, PRDs), the goal is to leverage AI for rapid generation of working components or solutions. The focus is on achieving ambitious goals rapidly.

- **Customer Collaboration over Contract Negotiation (Agile) vs. Vibe CEO as Ultimate Arbiter (Law Method):**

  - **Agile:** Involves continuous feedback from the customer.
  - **Law Method:** The "Vibe CEO" acts as the primary stakeholder and quality control ("QUALITY_CONTROL," "STRATEGIC_OVERSIGHT"), constantly reviewing and refining AI outputs, much like a highly engaged customer.

- **Responding to Change over Following a Plan (Agile) vs. Embrace Chaos & Adapt (Law Method):**

  - **Agile:** Values adaptability and responsiveness to new requirements.
  - **Law Method:** Explicitly encourages to "EMBRACE_THE_CHAOS," "ADAPT & EXPERIMENT," and acknowledges that "ITERATIVE_REFINEMENT" means it's "not a linear process." This directly mirrors Agile's flexibility.

- **Iterative Development & Incremental Delivery (Agile) vs. Task-based Implementation & Phased Value (Law Method):**

  - **Agile:** Work is broken down into sprints, delivering value incrementally.
  - **Law Method:** Projects are broken into Epics and Tasks, with "Developer Agents" implementing tasks one at a time. Epics represent "significant, deployable increments of value," aligning with incremental delivery.

- **Continuous Feedback & Retrospectives (Agile) vs. Iterative Refinement & Quality Control (Law Method):**
  - **Agile:** Teams regularly reflect and adjust processes.
  - **Law Method:** The "Vibe CEO" continuously reviews outputs ("QUALITY_CONTROL") and directs "ITERATIVE_REFINEMENT," serving a similar function to feedback loops and process improvement.

## Law Method - TOOLING AND RESOURCE LOCATIONS

Effective use of the Law Method relies on understanding where key tools, configurations, and informational resources are located and how they are used. The method is designed to be tool-agnostic in principle, with agent instructions and workflows adaptable to various AI platforms and IDEs.

- **Law Method Knowledge Base:** This document (`law-method-agent/data/law-method-kb.md`) serves as the central repository for understanding the Law Method, its principles, agent roles, and workflows.
- **Orchestrator Agents:** A key feature is the Orchestrator agent (AKA "Law Method Orchestrator"), a master agent capable of embodying any specialized agent role.
  - **Web Agent Orchestrator:**
    - **Setup:** Utilizes a Node.js build script (`build-web-agent.js`) configured by `build-web-agent.cfg.js`.
    - **Process:** Consolidates assets (personas, tasks, templates, checklists, data) from an `/law-method-agent` into a `build_dir`, default: `/build/`.
    - **Output:** Produces bundled asset files (e.g., `personas.txt`, `tasks.txt`), an `agent-prompt.txt` (from `composer_agent_prompt`), and an `agent-config.txt` (from `agent_cfg` like `web-Law-Method-composer-agent.cfg.md`).
    - **Usage:** The `agent-prompt.txt` is used for the main custom web agent instruction set (e.g., Gemini 2.5 Gem or OpenAI Custom GPT), and the other build files are attached as knowledge/files.
  - **IDE Agent Orchestrator (`ide-Law-Method-composer.md`):**
    - **Setup:** Works without a build step, dynamically loading its configuration.
    - **Configuration (`ide-Law-Method-composer.cfg.md`):** Contains a `Data Resolution` section (defining base paths for assets like personas, tasks) and `Agent Definitions` (Title, Name, Customize, Persona file, Tasks).
    - **Operation:** Loads its config, lists available personas, and upon user request, embodies the chosen agent by loading its persona file and applying customizations.
    - The `ide-Law-Method-composer` file contents can be used as the instructions for a custom agent mode. The agent supports a `*help` command that can help guide the user. The agent relies on the existence in the law-method-agent folder being at the root of the project.
    - The `ide-Law-Method-composer` is not recommended for generating tasks or doing development. While it CAN become those agents, its HIGHLY recommended to instead use the dedicated dev.ide.md or task-manager.ide.md as individual dedicated agents. The will use up less context overhead and are going to be used the most frequently.
- **Standalone IDE Agents:**
  - Optimized for IDE environments (e.g., Windsurf, Cursor), often under 6K characters (e.g., `dev.ide.md`, `task-manager.ide.md`).
  - Can directly reference and execute tasks.
- **Agent Configuration Files:**
  - `web-Law-Method-composer-agent.cfg.md`: Defines agents the Web Orchestrator can embody, including references to personas, tasks, checklists, and templates (e.g., `personas#pm`, `tasks#create-prd`).
  - `ide-Law-Method-composer.cfg.md`: Configures the IDE Orchestrator, defining `Data Resolution` paths (e.g., `(project-root)/law-method-agent/personas`) and agent definitions with persona file names (e.g., `analyst.md`) and task file names (e.g., `create-prd.md`).
  - `web-Law-Method-composer-agent.md`: Main prompt for the Web Orchestrator.
  - `ide-Law-Method-composer.md`: Main prompt/definition of the IDE Orchestrator agent.
- **Task Files:**
  - Located in `law-method-agent/tasks/` (and sometimes `law-method-agent/checklists/` for checklist-like tasks).
  - Self-contained instruction sets for specific jobs (e.g., `create-prd.md`, `checklist-run-task.md`).
  - Reduce agent bloat and provide on-demand functionality for any capable agent.
- **Core Agent Definitions (Personas):**
  - Files (typically `.md`) defining core personalities and instructions for different agents.
  - Located in `law-method-agent/personas/` (e.g., `analyst.md`, `pm.md`).
- **Project Documentation (Outputs):**
- **Project Briefs:** Generated by the Analyst agent.
- **Product Requirements Documents (PRDs):** Produced by the PM agent, containing epics and tasks.
- **UX/UI Specifications & Architecture Documents:** Created by Design Architect and Architect agents.
- The **POSM agent** is crucial for organizing and managing these documents.
- **Templates:** Standardized formats for briefs, PRDs, checklists, etc., likely stored in `law-method-agent/templates/`.
- **Data Directory (`law-method-agent/data/`):** Stores persistent data, knowledge bases (like this one), and other key information for the agents.

## Law Method - COMMUNITY AND CONTRIBUTIONS

The Law Method thrives on community involvement and collaborative improvement.

- **Getting Involved:**
  - **GitHub Discussions:** The primary platform for discussing potential ideas, use cases, additions, and enhancements to the method.
  - **Reporting Bugs:** If you find a bug, check existing issues first. If unreported, provide detailed steps to reproduce, along with any relevant logs or screenshots.
  - **Suggesting Features:** Check existing issues and discussions. Explain your feature idea in detail and its potential value.
- **Contribution Process (Pull Requests):**
  1. Fork the repository.
  2. Create a new branch for your feature or bugfix (e.g., `feature/your-feature-name`).
  3. Make your changes, adhering to existing code style and conventions. Write clear comments for complex logic.
  4. Run any tests or linting to ensure quality.
  5. Commit your changes with clear, descriptive messages (refer to the project's commit message convention, often found in `docs/commit.md`).
  6. Push your branch to your fork.
  7. Open a Pull Request against the main branch of the original repository.
- **Code of Conduct:** All participants are expected to abide by the project's Code of Conduct.
- **Licensing of Contributions:** By contributing, you agree that your contributions will be licensed under the same license as the project (MIT License).

### Licensing

The Law Method and its associated documentation and software are distributed under the **MIT License**.

Copyright (c) 2025 Brian AKA Law Method

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Law Method - ETHOS & BEST PRACTICES

- **CORE_ETHOS:** You are the "Vibe CEO." Think like a CEO with unlimited resources and a singular vision. Your AI agents are your high-powered team. Your job is to direct, refine, and ensure quality towards your ambitious goal. The method elevates "vibe coding" to advanced project planning.
- **MAXIMIZE_AI_LEVERAGE:** Push the AI. Ask for more. Challenge its outputs. Iterate.
- **QUALITY_CONTROL:** You are the ultimate arbiter of quality. Review all outputs.
- **STRATEGIC_OVERSIGHT:** Maintain the high-level vision. Ensure agent outputs align.
- **ITERATIVE_REFINEMENT:** Expect to revisit steps. This is not a linear process.
- **CLEAR_INSTRUCTIONS:** The more precise your requests, the better the AI's output.
- **DOCUMENTATION_IS_KEY:** Good inputs (briefs, PRDs) lead to good outputs. The POSM agent is crucial for organizing this.
- **KNOW_YOUR_AGENTS:** Understand each agent's role (see [AGENT ROLES AND RESPONSIBILITIES](#agent-roles-and-responsibilities) or below). This includes understanding the capabilities of the Orchestrator agent if you are using one.
- **START_SMALL_SCALE_FAST:** Test concepts, then expand.
- **EMBRACE_THE_CHAOS:** Pioneering new methods is messy. Adapt and overcome.
- **ADAPT & EXPERIMENT:** The Law Method provides a structure, but feel free to adapt its principles, agent order, or templates to fit your specific project needs and working style. Experiment to find what works best for you. **Define agile the Law Method way - or your way!** The agent configurations allow for customization of roles and responsibilities.

## AGENT ROLES AND RESPONSIBILITIES

Understanding the distinct roles and responsibilities of each agent is key to effectively navigating the Law Method workflow. While the "Vibe CEO" provides overall direction, each agent specializes in different aspects of the project lifecycle. The Law Method introduces Orchestrator agents that can embody these roles, with configurations specified in `web-Law-Method-composer-agent.cfg.md` for web and `ide-Law-Method-composer.cfg.md` for IDE environments.

- **Orchestrator Agent (Law Method Orchestrator):**

  - **Function:** The primary composer, initially "Law Method Orchestrator." It can embody various specialized agent personas. It handles general Law Method queries, provides oversight, and is the go-to when unsure which specialist is needed.
  - **Persona Reference:** `personas#Law-Method-Orchestrator` (Web) or implicitly the core of `ide-Law-Method-composer.md` (IDE).
  - **Key Data/Knowledge:** Accesses `data#law-method-kb-data` (Web) for its knowledge base.
  - **Types:**
    - **Web Orchestrator:** Built using a script, leverages large context windows of platforms like Gemini 2.5 or OpenAI GPTs. Uses bundled assets. Its behavior and available agents are defined in `web-Law-Method-composer-agent.cfg.md`.
    - **IDE Orchestrator:** Operates directly in IDEs like Cursor or Windsurf without a build step, loading persona and task files dynamically based on its configuration (`ide-Law-Method-composer.cfg.md`). The composer itself is defined in `ide-Law-Method-composer.md`.
  - **Key Feature:** Simplifies agent management, especially in environments with limitations on the number of custom agents.

- **Analyst:**

  - **Function:** Handles research, requirements gathering, brainstorming, and the creation of Project Briefs.
  - **Web Persona:** `Analyst (Mary)` with persona `personas#analyst`. Customized to be "a bit of a know-it-all, and likes to verbalize and emote." Uses `templates#project-brief-tmpl`.
  - **IDE Persona:** `Analyst (Larry)` with persona `analyst.md`. Similar "know-it-all" customization. Tasks for Brainstorming, Deep Research Prompt Generation, and Project Brief creation are often defined within the `analyst.md` persona itself ("In Analyst Memory Already").
  - **Output:** `Project Brief`.

- **Product Manager (PM):**

  - **Function:** Responsible for creating and maintaining Product Requirements Documents (PRDs), overall project planning, and ideation related to the product.
  - **Web Persona:** `Product Manager (John)` with persona `personas#pm`. Utilizes `checklists#pm-checklist` and `checklists#change-checklist`. Employs `templates#prd-tmpl`. Key tasks include `tasks#create-prd`, `tasks#correct-course`, and `tasks#create-deep-research-prompt`.
  - **IDE Persona:** `Product Manager (PM) (Jack)` with persona `pm.md`. Focused on producing/maintaining the PRD (`create-prd.md` task) and product ideation/planning.
  - **Output:** `Product Requirements Document (PRD)`.

- **Architect:**

  - **Function:** Designs system architecture, handles technical design, and ensures technical feasibility.
  - **Web Persona:** `Architect (Fred)` with persona `personas#architect`. Uses `checklists#architect-checklist` and `templates#architecture-tmpl`. Tasks include `tasks#create-architecture` and `tasks#create-deep-research-prompt`.
  - **IDE Persona:** `Architect (Mo)` with persona `architect.md`. Customized to be "Cold, Calculating, Brains behind the agent crew." Generates architecture (`create-architecture.md` task), helps plan tasks (`draft-task-from-epic.md`), and can update PO-level epics/tasks (`doc-sharding-task.md`).
  - **Output:** `Architecture Document`.

- **Design Architect:**

  - **Function:** Focuses on UI/UX specifications, front-end technical architecture, and can generate prompts for AI UI generation services.
  - **Web Persona:** `Design Architect (Jane)` with persona `personas#design-architect`. Uses `checklists#frontend-architecture-checklist`, `templates#front-end-architecture-tmpl` (for FE architecture), and `templates#front-end-spec-tmpl` (for UX/UI Spec). Tasks: `tasks#create-frontend-architecture`, `tasks#create-ai-frontend-prompt`, `tasks#create-uxui-spec`.
  - **IDE Persona:** `Design Architect (Millie)` with persona `design-architect.md`. Customized to be "Fun and carefree, but a frontend design master." Helps design web apps, produces UI generation prompts (`create-ai-frontend-prompt.md` task), plans FE architecture (`create-frontend-architecture.md` task), and creates UX/UI specs (`create-uxui-spec.md` task).
  - **Output:** `UX/UI Specification`, `Front-end Architecture Plan`, AI UI generation prompts.

- **Product Owner (PO):**

  - **Function:** Agile Product Owner responsible for validating documents, ensuring development sequencing, managing the product backlog, running master checklists, handling mid-sprint re-planning, and drafting user tasks.
  - **Web Persona:** `PO (Sarah)` with persona `personas#po`. Uses `checklists#po-master-checklist`, `checklists#task-draft-checklist`, `checklists#change-checklist`, and `templates#task-tmpl`. Tasks include `tasks#draft-task-from-epic`, `tasks#doc-sharding-task` (extracts epics and shards architecture), and `tasks#correct-course`.
  - **IDE Persona:** `Product Owner AKA PO (Curly)` with persona `po.md`. Described as a "Jack of many trades." Tasks include `create-prd.md`, `draft-task-from-epic.md`, `doc-sharding-task.md`, and `correct-course.md`.
  - **Output:** User Tasks, managed PRD/Backlog.

- **Task Manager:**

  - **Function:** Manages the detailed definition of tasks from Epics, oversees the completion of development tasks via checkboxes in `task-tmpl.md`, and is critical for logging changelogs, core dumps, and main task list updates under Law Method's direction.
  - **Web Persona:** `Task Manager (Bob)` with persona `personas#task-manager`. Described as "A very Technical Task Manager." Uses `checklists#change-checklist`, `checklists#task-dod-checklist`, `checklists#task-draft-checklist`, and `templates#task-tmpl`. Tasks: `tasks#checklist-run-task`, `tasks#correct-course`, `tasks#draft-task-from-epic`.
  - **IDE Persona:** `Task Manager (SallyTM)` with persona `task-manager.ide.md`. Described as "Super Technical and Detail Oriented," specialized in "Next Task Generation" (likely leveraging the `task-manager.ide.md` persona's capabilities).

- **Developer Agents (DEV):**
  - **Function:** Implement tasks one at a time. Can be generic or specialized.
  - **Web Persona:** `DEV (Dana)` with persona `personas#dev`. Described as "A very Technical Senior Software Developer."
  - **IDE Personas:** Multiple configurations can exist, using the `dev.ide.md` persona file (optimized for <6K characters for IDEs). Examples:
    - `Frontend Dev (DevFE)`: Specialized in NextJS, React, Typescript, HTML, Tailwind.
    - `Dev (Dev)`: Master Generalist Expert Senior Full Stack Developer.
  - **Configuration:** Specialized agents can be configured in `ide-Law-Method-composer.cfg.md` for the IDE Orchestrator, or defined for the Web Orchestrator. Standalone IDE developer agents (e.g., `dev.ide.md`) are also available.
  - **When to Use:** During the implementation phase, typically working within an IDE.

- **Researcher:**
  - **Function:** Conducts in-depth research on specific topics, technologies, or external documentation to provide necessary context and information for other agents (e.g., Analyst, PM, Architect).
  - **Web Persona:** `Researcher (Alice)` with persona `personas#researcher`. Uses `templates#research-summary-report-tmpl`. Tasks: `tasks#fetch-external-doc`, `tasks#create-deep-research-prompt`.
  - **IDE Persona:** `Researcher (BobR)` with persona `researcher.md`. Focuses on fetching external documentation and summarizing research.
  - **Typical Engagement:** Engaged when Analyst needs market data, PM needs competitive analysis, or Architect needs to evaluate new technologies.

- **GitHub Expert:**
  - **Function:** Manages GitHub repository operations, including creating feature branches, handling pull requests, and ensuring proper version control.
  - **Web Persona:** `GitHub Expert (Charlie)` with persona `personas#github-expert`. Uses `templates#pull-request-description-tmpl`. Tasks: `tasks#create-feature-branch`, `tasks#create-pull-request`.
  - **IDE Persona:** `GitHub Expert (DaveG)` with persona `github-expert.md`. Specializes in repository setup, branching strategies, and PR management.
  - **Typical Engagement:** Engaged after initial project creation for repo setup, when a new feature requires a dedicated branch, or for managing code merges.

## NAVIGATING THE Law Method WORKFLOW - INITIAL GUIDANCE

### STARTING YOUR PROJECT - ANALYST OR PM?

- Use Analyst if unsure about idea/market/feasibility or need deep exploration.
- Use PM if concept is clear or you have a Project Brief.
- Refer to [AGENT ROLES AND RESPONSIBILITIES](#agent-roles-and-responsibilities) (or section within this KB) for full details on Analyst and PM.

### UNDERSTANDING EPICS - SINGLE OR MULTIPLE?

- Epics represent significant, deployable increments of value.
- Multiple Epics are common for non-trivial projects or a new MVP (distinct functional areas, user journeys, phased rollout).
- Single Epic might suit very small MVPs, or post MVP / brownfield new features.
- The PM helps define and structure epics.

## GETTING STARTED WITH Law Method

This section provides guidance for new users on how to set up their project with the Law Method agent structure and manage artifacts.

### Initial Project Setup

To begin using the Law Method and its associated agents in your project, you need to integrate the core agent files:

- **Copy `law-method-agent` Folder:** The entire `law-method-agent` folder should be copied into the root directory of your project. This folder contains all the necessary personas, tasks, templates, and configuration files for the Law Method agents to function correctly.

### Exporting Artifacts from AI Platforms

Once an AI agent (like those in Gemini or ChatGPT) has generated a document (e.g., Project Brief, PRD, Architecture Document), you'll need to save it into your project:

- **Gemini:**
  - After the document is produced, click the `...` (more options) menu typically found near the response.
  - Select "Copy". The content will be copied as Markdown.
  - Paste this content into a new `.md` file within your project's `docs` folder (or a similar designated location).
  - **Passing to a new chat instance:** Gemini's chat interface may not directly support pasting Markdown with full fidelity in all scenarios.
    - You can paste the raw Markdown content directly.
    - Alternatively, save the content as a `.txt` file and paste from there.
    - For sharing or preserving formatting in Google Docs: Create a new Google Doc, right-click, and select "Paste without formatting" if pasting directly, or look for options to import/paste Markdown. Some browser extensions can facilitate Markdown rendering in Google Docs.
- **ChatGPT:**
  - ChatGPT generally handles Markdown well. You can copy the generated Markdown output directly.
  - Paste it into a `.md` file in your project's `docs` folder.
  - Sharing `.md` files or their content with new ChatGPT instances (e.g., by uploading the file or pasting the text) is typically straightforward.

### Document Sharding

Large documents like PRDs or Architecture Documents can become unwieldy for AI agents to process efficiently, especially in environments with context window limitations. The `doc-sharding-task.md` is designed to break these down:

- **Purpose:** The sharding task splits a large document (e.g., PRD, Architecture, Front-End Architecture) into smaller, more granular sections or individual user tasks. This makes it easier for subsequent agents, like the Task Manager or Dev Agents, to work with specific parts of the document without needing to process the entire thing.
- **How to Use:**
  1.  Ensure the large document you want to shard (e.g., `prd.md`, `architecture.md`) exists in your project's `docs` folder.
  2.  Instruct your active IDE agent (e.g., PO, Task Manager, or the Law Method Orchestrator embodying one of these roles) to run the `doc-sharding-task.md`.
  3.  You will typically specify the _source file_ to be sharded. For example: "Run the `doc-sharding-task.md` against `docs/prd.md`."
  4.  The task will guide the agent to break down the document. The output might be new smaller files or instructions on how the document is logically segmented.

### Utilizing Dedicated IDE Agents (Task Manager, Researcher, GitHub Expert, and Dev)

While the Law Method IDE Orchestrator can embody any persona, for common and intensive tasks like task generation (Task Manager), research (Researcher), GitHub operations (GitHub Expert), and code implementation (Dev), it's highly recommended to use dedicated, specialized agents:

- **Why Dedicated Agents?**
  - **Context Efficiency:** Dedicated agents (e.g., `task-manager.ide.md`, `researcher.md`, `github-expert.md`, `dev.ide.md`) are leaner as their persona files are smaller and more focused. This is crucial in IDEs where context window limits can impact performance and output quality.
  - **Performance:** Less overhead means faster responses and more focused interactions.
- **Recommendation:**
  - Favor using `task-manager.ide.md` for Task Manager tasks (like generating the next task).
  - Favor using `researcher.md` for research tasks.
  - Favor using `github-expert.md` for GitHub operations.
  - Favor using `dev.ide.md` for development tasks.
- **Creating Your Own Dedicated Agents:**
  - If your IDE supports more than a few custom agent modes (unlike Cursor's typical limit of 5 without paying for more), you can easily create your own specialized agents.
  - Take the content of a base persona file (e.g., `law-method-agent/personas/architect.md`).
  - Optionally, integrate the content of frequently used task files directly into this new persona file.
  - Save this combined content as a new agent mode in your IDE (e.g., `my-architect.ide.md`). This approach mirrors how the `task-manager.ide.md` agent is structured.

### When to Use the Law Method IDE Orchestrator

The Law Method IDE Orchestrator (`ide-Law-Method-composer.md` configured by `ide-Law-Method-composer.cfg.md`) provides flexibility but might not always be the most efficient choice.

- **Useful Scenarios:**
  - **Cursor IDE with Agent Limits:** If you're using an IDE like Cursor and frequently need to switch between many different agent personalities (Analyst, PM, Architect, etc.) beyond the typical free limit for custom modes, the Orchestrator allows you to access all configured personas through a single agent slot.
  - **Unified Experience (Gemini/ChatGPT Parity):** If you prefer to interact with the Law Method agent system in your IDE in the same way you would in a web UI like Gemini (using the Law Method Orchestrator to call upon different specialists), and you are not concerned about context limits or potential costs associated with larger LLM models that can handle the Orchestrator's broader context.
  - **Access to all Personas:** You want quick access to any of the defined agent personas without setting them up as individual IDE modes.
- **Potentially Unnecessary / Less Optimal Scenarios:**
  - **Simple Projects / Feature Additions (Caution Advised):** For very simple projects or when adding a small feature to an existing codebase, you _might_ consider a streamlined flow using the Orchestrator to embody the PM, generate a PRD with epics/tasks, and then directly move to development, potentially skipping detailed architecture.
    - In such cases, the PM persona might be prompted to ask more technical questions to ensure generated tasks are sufficiently detailed for developers.
    - **This is generally NOT recommended** as it deviates from the robust Law Method process and is not yet a fully streamlined or validated path. It risks insufficient planning and lower quality outputs.
  - **Frequent Task Manager/Dev Tasks:** As mentioned above, for regular task creation and development, dedicated Task Manager and Dev agents are more efficient due to smaller context overhead.

Always consider the trade-offs between the Orchestrator's versatility and the efficiency of dedicated agents, especially concerning your IDE's capabilities and the complexity of your project.

## SUGGESTED ORDER OF AGENT ENGAGEMENT (TYPICAL FLOW)

**NOTE:** This is a general guideline. The Law Method is iterative; phases/agents might be revisited.

1. **Analyst** - brainstorm and create a project brief.
2. **PM (Product Manager)** - use the brief to produce a PRD with high level epics and tasks.
3. **Design Architect UX UI Spec for PRD (If project has a UI)** - create the front end UX/UI Specification.
4. **Architect** - create the architecture and ensure we can meet the prd requirements technically - with enough specification that the dev agents will work consistently.
5. **Design Architect (If project has a UI)** - create the front end architecture and ensure we can meet the prd requirements technically - with enough specification that the dev agents will work consistently.
6. **Design Architect (If project has a UI)** - Optionally create a prompt to generate a UI from AI services such as Lovable or V0 from Vercel.
7. **PO**: Validate documents are aligned, sequencing makes sense, runs a final master checklist. The PO can also help midstream development replan or course correct if major changes occur.
8. **Researcher**: If Analyst, PM, or Architect needs external information, the Researcher can be engaged to fetch and summarize relevant documentation.
9. **GitHub Expert**: Engaged for repository setup after initial project creation, creating feature branches, and managing pull requests.
10. **Task Manager**: Generates detailed tasks from Epics, manages development task completion, and logs changelogs, core dumps, and main task list updates under Law Method's direction. This is generally done in the IDE after each task is completed by the Developer Agents.
11. **Developer Agents**: Implement tasks one at a time. You can craft different specialized Developer Agents, or use a generic developer agent. It is recommended to create specialized developer agents and configure them in the `ide-Law-Method-composer.cfg`.

## HANDLING MAJOR CHANGES

Major changes are an inherent part of ambitious projects. The Law Method embraces this through its iterative nature and specific agent roles:

- **Iterative by Design:** The entire Law Method workflow is built on "ITERATIVE_REFINEMENT." Expect to revisit previous steps and agents as new information emerges or requirements evolve. It's "not a linear process."
- **Embrace and Adapt:** The core ethos includes "EMBRACE_THE_CHAOS" and "ADAPT & EXPERIMENT." Major changes are opportunities to refine the vision and approach.
- **PO's Role in Re-planning:** The **Product Owner (PO)** is key in managing the impact of significant changes. They can "help midstream development replan or course correct if major changes occur." This involves reassessing priorities, adjusting the backlog, and ensuring alignment with the overall project goals.
- **Strategic Oversight by Vibe CEO:** As the "Vibe CEO," your role is to maintain "STRATEGIC_OVERSIGHT." When major changes arise, you guide the necessary pivots, ensuring the project remains aligned with your singular vision.
- **Re-engage Agents as Needed:** Don't hesitate to re-engage earlier-phase agents (e.g., Analyst for re-evaluating market fit, PM for revising PRDs, Architect for assessing technical impact) if a change significantly alters the project's scope or foundations.

## IDE VS UI USAGE - GENERAL RECOMMENDATIONS

The Law Method can be orchestrated through different interfaces, typically a web UI for higher-level planning and an IDE for development and detailed developer task generation. The most general recommendation is to do all document generation from the brief, PRD, Architecture, Design Architecture, and potentially UI Prompts. Also use the PO to run the full final checklist to ensure all documents are aligned with various changes. For example, did the architect discover something that requires an update to an epic or task sequence in the PRD? The PO will help you there. Once done, then export the documents to the IDE. If documents have been modified, you can ask the specific proper agents in Gemini or chatGPT to give you the final unredacted complete document. Save these into the docs folder of your project.

### CONCEPTUAL, PLANNING PHASES and TECHNICAL DESIGN

- **Interface:** Often best managed via a Web UI (leveraging the **Web Agent Orchestrator** with its bundled assets and `agent-prompt.txt`) or dedicated project management tools where composer agents can guide the process.
- **Agents Involved:**
  - **Analyst:** Brainstorming, research, and initial project brief creation.
  - **PM (Product Manager):** PRD development, epic and high-level story definition.
  - **Architect / Design Architect (UI):** Detailed technical design and specification.
  - **PO:** Checklist runner to make sure all of the documents are aligned.
- **Activities:** Defining the vision, initial requirements gathering, market analysis, high-level planning. The `web-Law-Method-composer-agent.md` and its configuration likely support these activities.

### DOCUMENTATION MANAGEMENT & IMPLEMENTATION PHASES

- **Interface:** Primarily within the Integrated Development Environment (IDE), leveraging specialized agents (standalone or via the **Law Method Agent Orchestrator** configured with `ide-Law-Method-composer.cfg.md`).
- **Agents Involved:**
  - "**PO or Task Manager or Law Method Orchestrator Agent:** Run the doc sharing task to split the large files that have been created (PRD, Architecture etc...) into smaller granular documents that are easier for the Task Manager and Dev Agents to work with.
  - **Task Manager:** Detailed task generation, backlog refinement, often directly in the IDE or tools integrated with it.
  - **Developer Agents:** Code implementation for tasks, working directly with the codebase in the IDE.
- **Activities:** Detailed architecture, front-end/back-end design, code development, testing, leveraging IDE tasks (see "LEVERAGING IDE TASKS FOR EFFICIENCY"), using configurations like `ide-Law-Method-composer.cfg.md`.

### Law Method FILES

Understanding key files helps in navigating and customizing the Law Method process:

- **Knowledge & Configuration:**
  - `law-method-agent/data/law-method-kb.md`: This central knowledge base.
  - `ide-Law-Method-composer.cfg.md`: Configuration for IDE developer agents.
  - `ide-Law-Method-composer.md`: Definition of the IDE composer agent.
  - `web-Law-Method-composer-agent.cfg.md`: Configuration for the web composer agent.
  - `web-Law-Method-composer-agent.md`: Definition of the web composer agent.
- **Task Definitions:**
  - Files in `law-method-agent/tasks/` or `law-method-agent/checklists/` (e.g., `checklist-run-task.md`): Reusable prompts for specific actions and also used by agents to keep agent persona files lean.
- **Agent Personas & Templates:**
  - Files in `law-method-agent/personas/`: Define the core behaviors of different agents.
  - Files in `law-method-agent/templates/`: Standard formats for documents like Project Briefs, PRDs that the agents will use to populate instances of these documents.
- **Project Artifacts (Outputs - locations vary based on project setup):**
  - Project Briefs
  - Product Requirements Documents (PRDs)
  - UX/UI Specifications
  - Architecture Documents
  - Codebase and related development files.

## LEVERAGING IDE TASKS FOR EFFICIENCY

### PURPOSE OF IDE TASKS

- **Reduce Agent Bloat:** Avoid adding numerous, rarely used instructions to primary IDE agent modes (Dev Agent, Task Manager Agent) or even the Orchestrator's base prompt. Keeps agents lean, beneficial for IDEs with limits on custom agent complexity/numbers.
- **On-Demand Functionality:** Instruct an active IDE agent (standalone or an embodied persona within the IDE Orchestrator) to perform a task by providing the content of the relevant task file (e.g., from `law-method-agent/tasks/checklist-run-task.md`) as a prompt, or by referencing it if the agent is configured to find it (as with the IDE Orchestrator).
- **Versatility:** Any sufficiently capable agent can be asked to execute a task. Tasks can handle specific functions like running checklists, creating tasks, sharding documents, indexing libraries, etc. They are self-contained instruction sets.

### EXAMPLES OF TASK FUNCTIONALITY

**CONCEPT:** Think of tasks as specialized, callable mini-agents or on-demand instruction sets that main IDE agents or the Orchestrator (when embodying a persona) can invoke, keeping primary agent definitions streamlined. They are particularly useful for operations not performed frequently. The `docs/instruction.md` file provides more details on task setup and usage.

Here are some examples of functionalities provided by tasks found in `law-method-agent/tasks/`:

- **`create-prd.md`:** Guides the generation of a Product Requirements Document.
- **`draft-task-from-epic.md`:** Helps in defining and creating the next task for development from an Epic.
- **`create-architecture.md`:** Assists in outlining the technical architecture for a project.
- **`create-frontend-architecture.md`:** Focuses specifically on designing the front-end architecture.
- **`create-uxui-spec.md`:** Facilitates the creation of a UX/UI Specification document.
- **`create-ai-frontend-prompt.md`:** Helps in drafting a prompt for an AI service to generate UI/frontend elements.
- **`doc-sharding-task.md`:** Provides a process for breaking down large documents into smaller, manageable parts.
- **`library-indexing-task.md`:** Assists in creating an index or overview of a code library.
- **`checklist-run-task.md`:** Executes a predefined checklist (likely using `checklist-mappings.yml`).
- **`correct-course.md`:** Provides guidance or steps for when a project needs to adjust its direction.
- **`create-deep-research-prompt.md`:** Helps formulate prompts for conducting in-depth research on a topic.

These tasks allow agents to perform complex, multi-step operations by following the detailed instructions within each task file, often leveraging templates and checklists as needed.
