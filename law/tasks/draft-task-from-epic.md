# Draft Task from Epic

## Purpose

To identify the next logical task based on project progress and epic definitions, and then to prepare a comprehensive, self-contained, and actionable task file using the `Task Template`. This task ensures the task is enriched with all necessary technical context, requirements, and acceptance criteria, making it ready for efficient implementation by a Developer Agent with minimal need for additional research.

## Inputs for this Task

- Access to the project's documentation repository, specifically:
  - `docs/index.md` (hereafter "Index Doc")
  - All Epic files (e.g., `docs/epic-{n}.md` - hereafter "Epic Files")
  - Existing task files in `docs/tasks/`
  - Main PRD (hereafter "PRD Doc")
  - Main Architecture Document (hereafter "Main Arch Doc")
  - Frontend Architecture Document (hereafter "Frontend Arch Doc," if relevant)
  - Project Structure Guide (`docs/project-structure.md`)
  - Operational Guidelines Document (`docs/operational-guidelines.md`)
  - Technology Stack Document (`docs/tech-stack.md`)
  - Data Models Document (as referenced in Index Doc)
  - API Reference Document (as referenced in Index Doc)
  - UI/UX Specifications, Style Guides, Component Guides (if relevant, as referenced in Index Doc)
- The `.law/templates/task-tmpl.md` (hereafter "Task Template")
- The `.law/checklists/task-draft-checklist.md` (hereafter "Task Draft Checklist")
- User confirmation to proceed with task identification and, if needed, to override warnings about incomplete prerequisite tasks.

## Task Execution Instructions

### 1. Identify Next Task for Preparation

- Review `docs/tasks/` to find the highest-numbered task file.
- **If a highest task file exists (`{lastEpicNum}.{lastTaskNum}.task.md`):**

  - Verify its `Status` is 'Done' (or equivalent).
  - If not 'Done', present an alert to the user:

    ```
    ALERT: Found incomplete task:
    File: {lastEpicNum}.{lastTaskNum}.task.md
    Status: [current status]

    Would you like to:
    1. View the incomplete task details (instructs user to do so, agent does not display)
    2. Cancel new task creation at this time
    3. Accept risk & Override to create the next task in draft

    Please choose an option (1/2/3):
    ```

  - Proceed only if user selects option 3 (Override) or if the last task was 'Done'.
  - If proceeding: Check the Epic File for `{lastEpicNum}` for a task numbered `{lastTaskNum + 1}`. If it exists and its prerequisites (per Epic File) are met, this is the next task.
  - Else (task not found or prerequisites not met): The next task is the first task in the next Epic File (e.g., `docs/epic-{lastEpicNum + 1}.md`, then `{lastEpicNum + 2}.md`, etc.) whose prerequisites are met.

- **If no task files exist in `docs/tasks/`:**
  - The next task is the first task in `docs/epic-1.md` (then `docs/epic-2.md`, etc.) whose prerequisites are met.
- If no suitable task with met prerequisites is found, report to the user that task creation is blocked, specifying what prerequisites are pending. HALT task.
- Announce the identified task to the user: "Identified next task for preparation: {epicNum}.{taskNum} - {Task Title}".

### 2. Gather Core Story Requirements (from Epic File)

- For the identified task, open its parent Epic File.
- Extract: Exact Title, full Goal/User Task statement, initial list of Requirements, all Acceptance Criteria (ACs), and any predefined high-level Tasks.
- Keep a record of this original epic-defined scope for later deviation analysis.

### 3. Gather & Synthesize In-Depth Technical Context for Dev Agent

- <critical_rule>Systematically use the Index Doc (`docs/index.md`) as your primary guide to discover paths to ALL detailed documentation relevant to the current story's implementation needs.</critical_rule>
- Thoroughly review the PRD Doc, Main Arch Doc, and Frontend Arch Doc (if a UI task).
- Guided by the Index Doc and the task's needs, locate, analyze, and synthesize specific, relevant information from sources such as:
  - Data Models Doc (structure, validation rules).
  - API Reference Doc (endpoints, request/response schemas, auth).
  - Applicable architectural patterns or component designs from Arch Docs.
  - UI/UX Specs, Style Guides, Component Guides (for UI tasks).
  - Specifics from Tech Stack Doc if versions or configurations are key for this task.
  - Relevant sections of the Operational Guidelines Doc (e.g., task-specific error handling nuances, security considerations for data handled in this task).
- The goal is to collect all necessary details the Dev Agent would need, to avoid them having to search extensively. Note any discrepancies between the epic and these details for "Deviation Analysis."

### 4. Verify Project Structure Alignment

- Cross-reference the task's requirements and anticipated file manipulations with the Project Structure Guide (and frontend structure if applicable).
- Ensure any file paths, component locations, or module names implied by the task align with defined structures.
- Document any structural conflicts, necessary clarifications, or undefined components/paths in a "Project Structure Notes" section within the task draft.

### 5. Populate Story Template with Full Context

- Create a new task file: `docs/tasks/{epicNum}.{taskNum}.task.md`.
- Use the Task Template to structure the file.
- Fill in:
  - Task `{EpicNum}.{TaskNum}: {Short Title Copied from Epic File}`
  - `Status: Draft`
  - `Task` (User Task statement from Epic)
  - `Acceptance Criteria (ACs)` (from Epic, to be refined if needed based on context)
- **`Dev Technical Guidance` section (CRITICAL):**
  - Based on all context gathered (Step 3 & 4), embed concise but critical snippets of information, specific data structures, API endpoint details, precise references to _specific sections_ in other documents (e.g., "See `Data Models Doc#User-Schema-ValidationRules` for details"), or brief explanations of how architectural patterns apply to _this task_.
  - If UI task, provide specific references to Component/Style Guides relevant to _this task's elements_.
  - The aim is to make this section the Dev Agent's primary source for _task-specific_ technical context.
- **`Tasks / Subtasks` section:**
  - Generate a detailed, sequential list of technical tasks and subtasks the Dev Agent must perform to complete the task, informed by the gathered context.
  - Link tasks to ACs where applicable (e.g., `Task 1 (AC: 1, 3)`).
- Add notes on project structure alignment or discrepancies found in Step 4.
- Prepare content for the "Deviation Analysis" based on discrepancies noted in Step 3.
