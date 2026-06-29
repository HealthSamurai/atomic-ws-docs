# Work with an agent

Atomic Workspace agents help turn clinical intent into a working application. They are most useful when you treat them like a product analyst and builder, not like a search box.

## The agent's role

The agent can:

- ask clarifying questions
- write a product vision
- build screens and application behavior
- inspect files, services, skills, and app state
- run checks
- fix errors
- explain what changed

You remain responsible for the clinical intent. The agent should not invent policy, clinical thresholds, or approval rules without your review.

In a project, the agent conversation sits beside the live preview. Use the conversation for requirements, changes, and debugging. Use the preview to judge whether the app actually works for the clinical task.

## Start with requirements

At the beginning, the agent asks questions one at a time. This is intentional. It keeps the first version focused.

Answer with real workflow details:

```text
Nurses use this after discharge. They need to see which patients missed the Day 3 check-in, which patients reported worse pain, and which patients need a call today.
```

If the agent asks about something you do not know yet, say so:

```text
We have not decided the exact risk threshold. Use a visible placeholder and mark it for clinical review.
```

## Review before build

Before implementation, the agent should show a product vision or plan. Review it like a clinical handoff:

- Is the user group correct?
- Is the workflow realistic?
- Are the data fields right?
- Are clinical risks visible?
- Is the first version small enough to test?
- Are assumptions clearly marked?

Do not approve vague plans. Ask for sharper wording before the build starts.

## Ask for changes

Small requests work better than broad ones.

Good:

```text
Add a missed-check-in status to the clinician dashboard.
```

Good:

```text
Rename "Risk" to "Recovery status" and show the reason next to each status.
```

Too vague:

```text
Make it more clinical.
```

## Ask the agent to show evidence

When the app changes, ask the agent to verify it:

```text
Show me where the Day 3, Week 1, Week 4, and Month 3 check-ins appear in the app.
```

or:

```text
Run through a patient with worsening pain and show what the clinician sees.
```

## Keep clinical decisions explicit

If the app includes scoring, alerts, reminders, or recommendations, ask the agent to list the assumptions.

Example:

```text
List every threshold used for the recovery status and mark which ones need clinical approval.
```

This keeps the prototype useful without hiding unfinished clinical governance work.

After the first build, use [Review and validate an app](review-and-validate.md) to test the result with realistic cases.
