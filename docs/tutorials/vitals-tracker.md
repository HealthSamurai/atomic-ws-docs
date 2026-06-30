# Build a vitals tracker

This tutorial walks through a vital signs tracking project for patients and clinicians.

By the end, you will have a patient view for recording vitals and a clinician view that shows recent readings, trends, and readings that need review.

## Before You Start

Use this tutorial when a care team needs to follow vital signs between visits or during a monitoring program.

Keep the first version narrow:

- one patient group
- one set of vital signs
- one entry flow
- one clinician review view
- one rule for readings that need review

For this tutorial, track blood pressure, heart rate, temperature, oxygen saturation, weight, and pain score.

## Create The Project

1. Open Atomic Workspace.
2. Select **New project**.
3. Choose **Patient Vital Signs Tracker** if templates are available.
4. Paste this prompt:

```text
Create a vital signs tracker for patients and clinicians.

Patients should record blood pressure, heart rate, temperature, oxygen saturation, weight, and pain score between visits.

Clinicians should see the latest reading, recent trends, and readings that need review. The first version should include a patient vitals entry form, a clinician patient view, and a simple needs-review status for abnormal or missing readings.
```

5. Select **Generate**.

## Define The First Review Rules

The builder may ask which readings count as normal or concerning.

Use draft thresholds if your team has not approved final rules. Make that visible:

```text
Use draft thresholds for the first version and mark them as needing clinical review. Show the threshold next to each needs-review reading.
```

For the tutorial, ask for these first rules:

- blood pressure above the selected draft threshold needs review
- fever needs review
- oxygen saturation below the selected draft threshold needs review
- missing readings for two expected days need review
- pain worsening by two or more points needs review

## Review The Patient Entry Flow

Open the patient view and enter a normal set of readings.

Check that:

- each vital has a clear label
- units are visible
- pain score explains the scale
- the patient can submit without reading clinical jargon
- the confirmation is short and clear

Then enter a second set with one concerning value, such as worse pain or low oxygen saturation.

## Review The Clinician View

Open the clinician view.

Check that the first screen shows:

- latest reading
- trend over recent readings
- status for normal or needs review
- reason for needs-review status
- timestamp or date of the reading

Ask for one improvement:

```text
Show the reason beside each needs-review status, such as low oxygen saturation, fever, worsening pain, or missing readings.
```

## Test Three Patient Scenarios

Use the preview with three realistic cases:

1. A patient with normal recent readings.
2. A patient with one abnormal reading.
3. A patient who has missed expected readings.

For each case, confirm that the clinician can answer:

- does this patient need attention now?
- why is this patient flagged?
- what changed since the last reading?
- what should the clinician open next?

## Continue The Loop

Keep the next change small.

Good next changes include:

- add a chart for blood pressure over time
- sort the review list by needs-review status
- add an empty state when no readings exist yet
- add a note field for patient context
- add a clinic-level view of patients needing review

Next, see [Create analytics and charts](../how-to/create-analytics-and-charts.md) or [App patterns](../explanation/app-patterns.md).
