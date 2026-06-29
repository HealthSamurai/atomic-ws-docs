# Create your first project

This guide walks through the first normal user flow: describe a clinical need, let the agent clarify it, and review the first working app.

## Before you start

You need access to Atomic Workspace and an AI agent already available for project work. If project creation says no agent is available, ask your Atomic Workspace administrator or project lead to enable one.

You should also have a concrete clinical or operational problem in mind. A good starting point is one workflow, one user group, and one outcome you want to improve.

## Create a project

1. Open Atomic Workspace.
2. Select **New project**.
3. Either describe what you want to build, or choose one of the templates.
4. Press **Generate**.

The home screen also has **Recent projects**. Use it to return to work you own under **My projects** or to open projects shared with you under **Shared with me**.

Good first prompts are specific but not technical:

```text
Create a post-surgery recovery tracker for patients and clinicians. Patients should report pain, mobility, and wellbeing after surgery. Clinicians should see recovery trends and alerts for worsening outcomes.
```

Avoid starting with implementation details such as frameworks, database tables, or deployment settings. The agent can handle those later. Your first job is to explain the clinical use case.

## Answer the agent's questions

After the project opens, the workspace is split into two main areas: the agent conversation on the left and the live application preview on the right. The agent will ask one question at a time. Answer in plain language.

Useful answers usually mention:

- who will use the app
- when they will use it
- what data they need to enter or review
- what decisions the app should support
- what should happen when something is abnormal, late, missing, or risky
- what the first version can safely leave out

When the agent has enough information, it writes a product vision for review. If you are done answering questions, say:

```text
stop
```

or:

```text
enough
```

## Review the product vision

Read the generated product vision before the agent builds. Check that it captures:

- the target users
- the workflow
- the key screens
- the clinical data involved
- the rules and exceptions
- the minimum useful first version

If something is wrong, tell the agent what to change. If it is correct, confirm that the agent should proceed.

You can also open **Files** and review `PRODUCT_VISION.md` there.

## Review the first app

When the app is built, use **Preview** to try it as a user would. If the project supports patient context, use the patient selector in the preview bar to test different cases.

Check:

- whether the first screen makes sense
- whether the app supports the real workflow
- whether patient and clinician views are clear
- whether abnormal or missing data is handled visibly
- whether the app uses understandable clinical language

Then ask the agent for changes. Keep each request small and concrete:

```text
Add a clinician summary card that shows the latest pain score, mobility score, and risk status.
```

or:

```text
Make the patient questionnaire shorter. Keep only pain, mobility, wound concerns, and free-text comments for the first version.
```

## Next steps

Use [Write a useful prompt](prompts.md) to improve your starting prompt, then use [Review and validate an app](review-and-validate.md) to test the result with realistic clinical scenarios.
