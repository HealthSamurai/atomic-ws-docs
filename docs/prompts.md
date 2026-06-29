# Write a useful prompt

A useful Atomic Workspace prompt describes the clinical job, not the software architecture.

The agent needs enough context to ask better questions and build the right first version. It does not need a complete requirements document at the start.

## Prompt structure

Use this shape:

```text
Create a [kind of app] for [users] who need to [job].

It should help them [main workflow].

The first version should include [screens, data, rules, or outputs].
```

Example:

```text
Create a patient intake app for clinics. Patients should complete intake before a visit, and clinicians should review the submitted information before the appointment.

The first version should collect demographics, contact details, reason for visit, current symptoms, medications, allergies, medical history, and consent.
```

## Good prompts

### Patient intake

```text
Create a patient intake app for clinics and hospitals. Patients should complete intake before or during a visit. Clinicians should review submitted forms in a structured view before the appointment.
```

### Vital signs tracker

```text
Create a vital signs tracker. Patients should record blood pressure, heart rate, temperature, oxygen saturation, weight, and pain score. Clinicians should see trends and abnormal values.
```

### Clinical data viewer

```text
Create a clinical data viewer for providers. It should show demographics, conditions, allergies, medications, vitals, labs, encounters, notes, and imaging reports in a clear patient summary.
```

### Decision support

```text
Create a clinical decision support app for providers. It should show medication interaction alerts, abnormal vital warnings, preventive care reminders, and care gap alerts that clinicians can acknowledge or dismiss.
```

### PROMs follow-up

```text
Create a patient-reported outcomes app. Care teams should send questionnaires, track completion, review results, and see patients who need follow-up.
```

### Patient engagement workflow

```text
Create a patient engagement workflow app for care teams. It should support follow-up activities, in-app reminders, task tracking, and a dashboard for participation and completion.
```

### Clinical calculator

```text
Create a clinical calculator app for providers. Include common scores, simple input forms, automatic calculations, and clear result interpretation.
```

### Analytics dashboard

```text
Create a healthcare analytics dashboard for clinical and operational teams. It should show population insights, quality metrics, outcomes, completion rates, care gaps, and filters by clinic, provider, and date.
```

## What to include

Include the clinical context:

- care setting
- user roles
- patient group
- key decisions
- data to collect or show
- rules for abnormal, late, missing, or high-risk cases
- what the first version should prove

## What to avoid

Do not start with:

- database schema
- UI framework
- hosting instructions
- generic requests such as "make a dashboard"
- a long list of unrelated features

For patient outreach, describe the workflow inside the app unless your organization has already enabled external messaging. For example, say "create a follow-up queue for staff" instead of assuming SMS or email delivery.

## Improve a weak prompt

Weak:

```text
Make a dashboard for surgery patients.
```

Better:

```text
Create a recovery tracking app for post-surgery patients. Patients should report pain, mobility, wound concerns, and wellbeing after surgery. Clinicians should see recovery trends, missed check-ins, and patients whose symptoms are getting worse.
```

Next, use [Work with an agent](agent-workflow.md) to turn the prompt into reviewed requirements.
