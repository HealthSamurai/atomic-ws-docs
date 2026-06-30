# Build a patient intake app

This tutorial walks through a pre-visit intake project for a clinic.

By the end, you will have a patient-facing intake form and a provider view for reviewing submitted intake details before the visit.

## Before You Start

Use this tutorial when your team needs patients to provide information before an appointment.

Keep the first version small:

- one clinic or care setting
- one visit type
- one patient intake form
- one provider review view
- one clear next action after review

For this tutorial, use a new adult primary-care visit.

## Create The Project

1. Open Atomic Workspace.
2. Select **New project**.
3. Choose **Patient Intake Flow** if templates are available.
4. Paste this prompt:

```text
Create a pre-visit patient intake app for adult primary-care visits.

Patients should complete intake before a new visit. The clinic team should review submitted intake details before the appointment.

The first version should include a patient intake form and a provider review view. Collect reason for visit, current symptoms, medications, allergies, medical history, preferred contact method, and consent acknowledgement.
```

5. Select **Generate**.

## Shape The Form

The builder may ask which fields are required, which words patients should see, and what should appear in the review view.

Answer with real clinic rules when you know them:

- reason for visit is required
- medications can be free text in the first version
- allergies should ask for reaction if known
- consent acknowledgement should appear before submission
- provider review should highlight missing required answers

If the team has not approved the final form wording, say:

```text
Use simple draft wording for the patient questions and mark the form text for clinical review.
```

## Review The Patient Form

When the first version appears, open the patient view.

Complete the form as a patient would:

1. Enter a clear reason for visit.
2. Add one medication.
3. Add one allergy.
4. Leave one optional field blank.
5. Submit the form.

Check that:

- required questions are obvious
- patient wording is plain
- the submit action is easy to find
- the confirmation explains what happens next
- optional missing details do not block submission

## Review The Provider View

Return to the provider view.

Open the submitted intake and check that the reviewer can quickly see:

- reason for visit
- symptoms
- medications
- allergies
- missing required details
- consent acknowledgement

Ask for one provider-facing improvement:

```text
Add a compact intake summary at the top of the provider view: reason for visit, allergies, medications, and missing required details.
```

## Test A Second Patient

Try one more patient example before expanding the project.

Use a patient who reports:

- chest discomfort in the reason for visit
- no known allergies
- no current medications
- one missing contact preference

Ask the builder:

```text
Show how this intake appears to the clinic team and make any urgent or missing details easy to notice.
```

## Continue The Loop

Add only one visible improvement at a time.

Good next changes include:

- split medication details into name, dose, and frequency
- add a review status for not reviewed, reviewed, and needs clarification
- add a clinic queue sorted by appointment date
- add a patient-friendly explanation before sensitive questions

Next, learn how to [create forms](../how-to/create-forms.md) or look up more starting points in the [Template catalog](../reference/template-catalog.md).
