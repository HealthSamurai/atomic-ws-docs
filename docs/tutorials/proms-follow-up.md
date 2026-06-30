# Build a PROMs follow-up app

This tutorial walks through a patient-reported outcomes project for a care team.

By the end, you will have a questionnaire, completion tracking, and a review view for submitted results.

## Before You Start

Use this tutorial when a team wants patients to report symptoms, function, wellbeing, or recovery progress after care.

Keep the first version focused:

- one outcome questionnaire
- one patient group
- one follow-up timing
- one care-team review view
- one rule for missed or concerning responses

For this tutorial, build a two-week follow-up after orthopedic surgery.

## Create The Project

1. Open Atomic Workspace.
2. Select **New project**.
3. Choose **PROMs Outreach** if templates are available.
4. Paste this prompt:

```text
Create a patient-reported outcomes follow-up app for orthopedic surgery patients.

Patients should complete a two-week follow-up questionnaire about pain, mobility, wound concerns, medication side effects, and overall recovery.

The care team should see completion status, submitted answers, and patients who missed the questionnaire or reported concerning responses. The first version should include a patient questionnaire, a care-team queue, and a submitted-response review view.
```

5. Select **Generate**.

## Shape The Questionnaire

Answer the builder questions in patient-centered language.

For the first version, ask for:

- pain score from 0 to 10
- mobility compared with discharge
- wound concern yes or no
- medication side effects yes or no
- free-text recovery concern
- overall recovery worse, same, or better

If your team already uses a standard questionnaire, say:

```text
Use our standard orthopedic two-week follow-up questionnaire. If the exact source is not available in the project, create a draft version and mark it for clinical review.
```

## Review The Patient Questionnaire

Open the patient view.

Complete the questionnaire once as a patient with normal recovery.

Check that:

- the questions are short
- the answer choices are understandable
- required answers are clear
- the patient can review before submitting
- the confirmation does not promise a specific response time unless your team has approved it

## Review The Care-Team Queue

Open the provider view.

Confirm that the queue separates:

- completed normal questionnaires
- missed questionnaires
- concerning responses

Ask for one queue improvement:

```text
Move missed questionnaires and concerning responses above normal completed questionnaires. Show the reason each row needs review.
```

## Review Submitted Results

Open a submitted questionnaire.

Check that the care team can quickly see:

- date submitted
- pain score
- mobility answer
- wound concern
- side effects
- overall recovery
- free-text concern

Ask for one review improvement:

```text
Add a short result summary at the top: recovery status, reason for review, and the most important patient-reported details.
```

## Test A Concerning Scenario

Use a patient who reports:

- worse recovery than expected
- pain score of 8
- wound concern
- a free-text concern about swelling

Ask the builder:

```text
Show what the care team sees for this response and make the reason for review visible on both the queue and detail view.
```

## Continue The Loop

Good next changes include:

- add a trend view for repeated questionnaires
- add a reviewer status for new, reviewed, and follow-up needed
- add a patient-facing explanation before the questionnaire
- add a clinical copilot that summarizes the submitted response and lists the facts it used

Next, see [Create forms](../how-to/create-forms.md) or [Create care workflows](../how-to/create-care-workflows.md).
