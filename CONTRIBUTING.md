# EthicalMatch Documentation Contribution Guide
*This document is incomplete. Check back later, or hop into the [community discord](https://discord.gg/P7qfVuqMXz) to participate in our initial discussions*

This document outlines how to contribute to both the technical documentation and the general resources that help the project run smoothly. Whether you’re a programmer or not, your contributions are essential to keeping EthicalMatch a focused, honest, and well-documented project.

( #todo *move to beginning of tech documentation* )
## Table of Contents

1. [Overview](#overview)
1. [Non-Code Contributions](#non-code-contributions)
1. [Technical Documentation Contributions](#technical-documentation-contributions)
1. [General Contribution Guidelines](#general-contribution-guidelines)
1. [First Time Contributing to Open Source?](#first-timers)
## Overview
EthicalMatch is committed to a documentation-first workflow that keeps information **ahead of code**. This approach enables non-programmers to participate meaningfully in the design process and gives developers a clear, pre-defined structure to work from.

Our repository is structured to support both technical and non-technical documentation:
- **Technical Documentation**: Clear descriptions of how features function, guides & examples on how to use them, and status tracking for the implementation of features in the product itself.
- **Non-Code Documentation**: Onboarding materials, guides for various roles, resources for involvement, and other documents that support the community and project operations.

## General Contribution Guidelines
#### Use (#todo) for Partial Contributions
If you’re contributing to a section but can’t complete it, leave a (#todo) comment where necessary, with a brief note on why it’s incomplete.
Incomplete sections and (#todo) notes encourage others to build on what you’ve started, helping keep ideas flowing even if they’re not fully formed.

> [!Example]
> "This is where we'll do a thing! ( #todo I don't know the exact method we should use here )"
## Non-Code Contributions
Non-programmer's provide a vital perspective to EthicalMatch. Your work can shape how the project runs, help onboard new members, and keep processes smooth and clear. Here’s how you can contribute:

1. **Reviewing and Enhancing**: Offer feedback on existing documentation, propose edits for clarity, and suggest resources that may be helpful for the team.
1. **Onboarding and Resources**: Review and add to onboarding guides for new roles, community guidelines, and participation resources.
1. **Process Improvements**: Help document effective workflows, communication strategies, or other practices to improve project management.

To contribute to these areas, please open a **Documentation Change Issue** and describe what you’re adding or improving. ( #todo this is inaccurate )

## Technical Documentation Contributions
If you’re contributing to the technical documentation for a code-based feature, please follow these guidelines:
### Workflow for New Features and Issues

1. **Feature Request Issue Creation**: All new ideas or significant changes should begin with a **Feature Request** issue. This creates a space for discussion and review.
1. **Documentation Design**: Approved features will enter the design stage, where documentation is drafted to describe the planned implementation. This can be done 
1. **Tracking Code Implementation Progress**: Each feature’s documentation will include a **Progress Label** to indicate its implementation status in the code.

## Contributing through Issues
In this repository, we use two main issue templates:
- **[Documentation Change](https://github.com/EthanGunter/EthicalMatch-docs/issues/new?assignees=&labels=enhancement&projects=&template=documentation-change.md&title=)**: Use this template for edits, updates, or minor changes to existing documentation. This can include formatting fixes, adding examples, or clarifying sections.
- **[Feature Request](https://github.com/EthanGunter/EthicalMatch-docs/issues/new?assignees=&labels=feature&projects=&template=feature_request.md&title=)**: Any new ideas or significant feature changes should go through a Feature Request issue. Contributors can join the discussion to refine the concept and suggest improvements. After approval, it moves into design.

 Feature Requests will go through the following stages:
1. **Review**: A submitted feature request is tagged and reviewed by our most active contributors.
1. **Design and Documentation**: Once approved, the feature enters a design phase where contributors discuss implementation details and draft the initial documentation.
1. **Development and Status Labelling**: New documentation must include a progress label with the starting status of `0%`. This label will be updated as each section is completed to track progress and keep the status of the project as transparent as possible.

### Development Status Tracking
Each documentation section will have a status label that indicates the progress percentage of each section. This make it clear what work needs to be done at a glance. Format it like so:
## Feature Header
![35%](https://progress-bar.xyz/35)
*Important documentation!*
```
## Feature Header
![35%](https://progress-bar.xyz/35%)
*Important documentation!*
```

> [!Note]
> While the sentiment here is to maintain the sovereignty of the documentation as the sole source of truth, keeping these updated with every code update is a real pain. If you have an idea how to automate this, weigh in on [the github issue](https://github.com/EthanGunter/EthicalMatch-docs/issues/2).

# Contribution Workflow
#todo This is here to delete a redundant file. It's still an unfinished concept, and will need updating and integrating with this document. I do like the high-level overview, however, and it might be a good idea to keep this info together (and as a flow chart 😎)
1. Idea/Feature request filed
1. Documentation created to fulfill the needs of that feature
	Review: ensure documentation fully addresses the feature requested, and considers edge cases
1. Feature_Dev branch created
	The actual code is written here without much oversight. The idea is to allow freedom to explore different specific implementations to figure out what works best.
	Review: Does the new code adhere to the documentation updates?
1. Feature_Test branch created
	Tests written to cover each item mentioned in the documentation
1. Final Pull-Request and merge with production