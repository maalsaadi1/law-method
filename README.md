# Law Method

This repository contains the "Law Method" project, a structured yet flexible framework designed to plan, execute, and manage software projects using a team of specialized AI agents. It aims to elevate "vibe coding" to advanced project planning by leveraging AI as a high-powered team.

This workflow is made for roocode extension. It utilizes the custom modes roocode uses.

## Project Structure

The core of the Law Method resides in the `law/` directory, which contains:
- `law/checklists/`: Checklists for various stages of the project.
- `law/data/`: Knowledge base and technical preferences.
- `law/personas/`: Definitions for different AI agent roles.
- `law/tasks/`: Task definitions and workflows.
- `law/templates/`: Templates for project documents like PRDs, architecture, etc.

## Key Concepts

- **Vibe CEO'ing:** Embracing chaos and directing AI agents as a high-powered team.
- **Specialized AI Agents:** Different AI roles (Analyst, PM, Architect, Dev, etc.) for specific project phases.
- **Iterative Refinement:** The process is designed for continuous adaptation and improvement.
- **Config-Driven:** Agent behaviors and tasks are defined by configuration files.

## Getting Started

To use Law-method follow these steps:
1. Clone the repo to the desired project:
   `git clone https://github.com/maalsaadi1/law-method.git`
2. Move the `law` folder and `.roomodes` file to the main path of your project.
3. In VS Code, press `Ctrl + P` (Windows) or `Cmd + P` (Mac) and choose "Reload Window".
4. Use the `Composer` persona as the main AI agent.

Roocode will then use the custom modes defined in `.roocode`.

For more detailed information, refer to the documentation within the `law/` directory, especially `law/data/law-method-kb.md`.
