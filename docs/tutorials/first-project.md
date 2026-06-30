# Build your first clinical app

This tutorial walks through one complete first project: a small post-discharge follow-up app for a care team.

By the end, you will have a working first version you can try in the project preview.

## Before You Start

You need access to Atomic Workspace and one clinical workflow idea.

Keep the first project narrow. A useful first version has:

- one patient group
- one care team or reviewer group
- one workflow
- one decision the app should support

For this tutorial, use post-discharge follow-up.

## Create The Project

The **New project** screen gives you a prompt box and templates for common clinical apps.

![New project screen with the prompt box and healthcare app templates](../../assets/screenshots/new-project-templates.avif)

1. Open Atomic Workspace.
2. Select **New project**.
3. Paste this prompt:

```text
Create a post-discharge follow-up app for a care team.

Patients should complete a short check-in after discharge. Nurses should see which patients completed the check-in, which patients missed it, and which patients reported worsening symptoms.

The first version should include a patient check-in form, a nurse work queue, and a simple status for normal, missed, and needs review.
```

4. Select **Generate**.

## Answer The Questions

The project builder asks questions to clarify the workflow. Answer in plain language.

Good answers name the real clinical details:

- who fills the form
- when the check-in should happen
- what symptoms matter
- what counts as normal, missing, or concerning
- who reviews the result
- what can wait until later

If you do not know a clinical rule yet, say that directly:

```text
We have not approved the exact risk threshold. Use a visible placeholder and mark it for clinical review.
```

When the builder has enough information, it writes an app plan. If the questions are no longer useful, say `enough` or `stop`.

## Check The App Plan

Read the app plan before the app is built.

Check that it names:

- target users
- patient group
- workflow steps
- data the app collects or shows
- clinical rules and assumptions
- first-version scope

If something is wrong, ask for a correction before the build starts:

```text
Change the reviewer from physicians to discharge nurses. Keep physicians out of the first version.
```

If it is right, confirm that the builder should continue.

## Try The First Version

When the first app appears, use the preview as a real user would.

Start with the provider view:

1. Choose a patient context if the preview offers one.
2. Open the nurse work queue.
3. Confirm that the queue shows completed, missed, and needs-review patients.
4. Open one patient or submitted response.
5. Check that the next action is clear.

Then review the patient-facing part if the project includes one:

1. Open the patient view.
2. Complete the check-in form.
3. Submit the form.
4. Return to the provider view and confirm the result appears.

## Ask For One Improvement

Keep the first change small. For example:

```text
Add a reason next to each needs-review status: worsening pain, new fever, missed check-in, or free-text concern.
```

After the change appears, try it with another patient example.

## Continue The Loop

Repeat the same loop:

1. ask for one visible change
2. review it in the preview
3. test a realistic case
4. correct the clinical language, assumptions, or next action

Next, try another tutorial: [Build a patient intake app](patient-intake.md), [Build a vitals tracker](vitals-tracker.md), or [Build a PROMs follow-up app](proms-follow-up.md).
