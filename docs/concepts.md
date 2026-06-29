# Key concepts

This page defines the main Atomic Workspace terms normal users see in the product.

## Project

A project is the shared place where your team builds and reviews one clinical application idea.

Projects can be created from a prompt or template. A project has its own app preview, files, services, agent conversation, and healthcare data sandbox.

The project list separates work into **My projects** and **Shared with me**. Project cards show the name, thumbnail, status, owner, created date, and available actions.

## Template

A template is a starting point for a common healthcare app idea. Atomic Workspace currently offers templates such as patient intake, vital signs tracking, clinical data viewer, decision support, PROMs outreach, patient engagement workflow, clinical calculator, and analytics report.

## Clinical application

A clinical application is the app being built inside a project.

Examples:

- recovery tracker
- patient intake app
- vital signs tracker
- clinical data viewer
- quality dashboard

The application belongs to the project team. Atomic Workspace provides the environment for building and reviewing it.

## Agent

An agent is an AI collaborator connected to the project. It can clarify requirements, write a product vision, build the app, inspect errors, and make changes.

The agent is not the clinical owner. Users still review requirements, clinical rules, thresholds, and approval decisions.

## Product vision

The product vision is the short project document that captures what the app should do before implementation begins.

It should describe users, workflow, data, rules, and first-version scope. Review it before approving the build.

## FHIR sandbox

Each project runs against a FHIR-native healthcare data environment. This lets the team build and review apps using healthcare data structures instead of fake generic data models.

For normal users, the important point is simple: the app can be tested in a healthcare-shaped environment before production.

## SMART app

A SMART app is a healthcare application that can launch from a FHIR-compliant EHR with patient and practitioner context.

Atomic Workspace is designed to help teams move toward SMART on FHIR apps when the project is ready for production planning.

## Preview

The preview is the live app view inside the project. It appears beside the agent conversation and includes app navigation controls, patient context when available, and a link to open the app in a separate tab.

## EHR simulator

The EHR simulator lets you review launch context, patient selection, practitioner identity, and app permissions without needing a production EHR.

## Services

Services are the running parts of the project. Most users only need them when the preview is starting, stopped, or failed.

## Files

Files contain the app, generated documents, and project artifacts. Normal users usually review files such as the product vision, clinical content, forms, or app notes. Developers may inspect code when deeper changes are needed.

## Skills

Skills are reusable guidance the agent can use while building the app. Healthcare-focused skills can guide FHIR, questionnaires, charts, and Aidbox-specific work.

## Aidbox

Aidbox is the healthcare data backend available inside the project. Analysts and developers can use it to inspect FHIR data when app behavior needs deeper validation.

## Published project

A published project is a project that is ready for a broader review or deployment path. Publication does not replace clinical, security, compliance, or operational approval.

For the first user flow, see [Create your first project](get-started.md).
