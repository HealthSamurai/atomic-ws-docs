# Review and validate an app

Atomic Workspace is useful because you can review a working app, not just a document. Use the workspace to test whether the app supports the real clinical workflow.

## Use the preview

The **Preview** tab shows the live app. Use it to walk through the main workflow as a clinician or care team member.

Check:

- the screen starts with the right task
- important patient or workflow context is visible
- status labels are clear
- actions are easy to find
- abnormal, missing, or late items are not hidden

If the app supports a patient view, use **Patient Preview** to review the patient-facing experience.

## Use patient context

When patient context is available, select different patients in the preview bar. Test at least:

- a normal case
- a high-risk or abnormal case
- a patient with missing data
- a patient with multiple recent events

The goal is not to prove every edge case. The goal is to find whether the app handles common clinical variation safely enough for the next review.

## Check app launch context

For SMART-style apps, check the launch context shown around the preview:

- which patient is selected
- which practitioner is launching the app
- what permissions the app asks for
- whether the app opens with the expected context

If the project imports patients from an external FHIR server, confirm that the imported patients appear in the patient picker before reviewing the app.

## Review services and logs

If the preview is unavailable, open **Services**.

Common states:

- **Starting**: wait and refresh the preview.
- **Stopped**: start the app service.
- **Failed**: open service logs and ask the agent to fix the error.
- **Running with no preview**: the app may not declare a preview port yet.

Normal users do not need to debug infrastructure. A useful request is:

```text
The preview is unavailable. Check the service logs and fix the app so I can open the provider view.
```

The service list shows the running parts of the project, such as the app, workers, or optional services. Treat it as a status panel unless you are deliberately starting or stopping a service.

## Review files only when needed

The **Files** tab is useful when you want to inspect generated documents, app copy, or configuration. You can also download the project files from this tab. You do not need to read code to validate a clinical workflow.

Good files to review:

- `PRODUCT_VISION.md`
- README or usage notes
- clinical content
- generated forms
- app manifest or permissions summary, when relevant

## Review skills and healthcare data

The **Skills** tab shows the guidance available to the agent, such as FHIR, Questionnaire, charting, or Aidbox guidance. This helps explain what patterns the agent can use.

The **Aidbox** tab opens the project healthcare data backend. Most clinical reviewers do not need it for routine app review, but it can help analysts and developers inspect the underlying FHIR data.

## Validate with scenarios

Use scenario-based review. Describe a realistic patient or workflow and ask the agent to exercise it.

Example:

```text
Test a post-surgery patient who misses the Week 1 check-in and reports worse pain at Week 4. Show what the clinician dashboard displays.
```

Useful validation scenarios include:

- normal completion
- missed follow-up
- abnormal result
- duplicate or conflicting information
- patient with limited history
- clinician dismisses or acknowledges a recommendation

## Decide what happens next

After review, put the project into one of these states:

- continue iterating in the workspace
- prepare for stakeholder review
- prepare for clinical, security, or compliance review
- stop the idea because the workflow is wrong or not worth building

Atomic Workspace helps you get to that decision faster. It does not remove the decision.

For term definitions, see [Core concepts](concepts.md). To improve the next iteration, go back to [Work with an agent](agent-workflow.md).
