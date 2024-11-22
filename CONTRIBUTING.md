# The Contribution Process Overview
## Change Starts with Documentation
At EthicalMatch, every new idea, from app features to marketing policies, begins with documentation. Why?
1. Documentation will *always* reflect the current state of the project
1. Clearly defined ideas make implementation smoother for developers
1. It gives autonomy to participants to learn and work at their own pace

## Use GitHub Issues to Propose Changes
All contributions start with a GitHub issue. This provides an avenue for conversation about your idea before any changes are made, and enables tracking of progress and prioritizing the interests of the community.  
The two issue templates you can open are:
- **[Documentation Change](https://github.com/Ethical-Commons-Project/EthicalMatch-docs/issues/new?assignees=&labels=enhancement&projects=&template=documentation-change.md&title=)**: For updates, clarifications, or new resources in the repository
- **[Feature Request](https://github.com/Ethical-Commons-Project/EthicalMatch-docs/issues/new?assignees=&labels=feature&projects=&template=feature_request.md&title=)**: For new functionality or significant changes requiring technical design and implementation

## Pull-Request Reviews and Approvals
If you'd like to add or modify a document yourself, that process involves making a pull request (PR). Before making your changes an official part of the project, pull requests undergo a review process to ensure quality, alignment with project goals, and adherence to our standards.
- **General Contributions** require approval from an authorized [area expert](https://github.com/Ethical-Commons-Project/EthicalMatch-docs/issues/8)
- **Technical Contributions** have a more involved process, detailed below

# Technical Documentation Process
## Documentation First?!
You may hear "documentation-first" and shudder, recalling the rigidity of [TDD](https://en.wikipedia.org/wiki/Test-driven_development) or the seemingly redundant drudgery of documenting existing code. With EthicalMatch, our documentation process is designed to be the opposite:  
- **It reduces your design workload.** By collaborating on plain-English documentation to start, we give you a roadmap without locking you into rigid implementation details.
- **It simplifies post-implementation documentation.** Because the initial idea is already described, updating the documentation becomes as simple as translating code to English, or providing usage examples ( #todo which is a likely candidate for automation… )  

By structuring documentation this way, we aim to reduce cognitive load at every stage, allowing you to focus on building while still ensuring clarity for future contributors.

## Workflow for Technical Contributions
The following is the simplified workflow for code contributions to EthicalMatch:
1. 💡 A `Feature Request` GitHub issue is created
	-  The `#valid-feature` tag is applied, giving the feature the green-light
1. 📝 Documentation is collaboratively drafted on a separate branch
	- Once a consensus is made, it gets merged with the main branch
2. 🚀The feature gets implemented in its relevant source-code repository
	- Each repository has its own contribution rules and expectations
3. 💯The docs are updated one last time to reflect completion status and flesh out specifics
> #todo Tests are not yet part of the pipeline, but they need to be. Look at [issue #7](https://github.com/Ethical-Commons-Project/EthicalMatch-docs/issues/7) regarding auto-written test tooling
## Breaking it down
### 1. Feature Request GitHub Issue Creation:
Every new feature or significant change starts with a [Feature Request Github Issue](https://github.com/Ethical-Commons-Project/EthicalMatch-docs/issues/new?assignees=&labels=feature&projects=&template=feature_request.md&title=). This provides problem information, and a proposed solution. Once the GitHub issue is tagged with \#valid-feature by one of our [authorized devs](https://github.com/Ethical-Commons-Project/EthicalMatch-docs/issues/8), it will get added to the [Feature Development Project](https://github.com/orgs/Ethical-Commons-Project/projects/2), and be opened for discussion and design.
### 2. Draft Documentation Collaboration:
Once a feature is accepted, it will be put in the [feature draft list](https://github.com/orgs/Ethical-Commons-Project/projects/2/views/5?filterQuery=status%3A%22drafting%22). Once in this list, a branch named "Draft-Feature-#X" and a PR for that branch will automatically be created. The comments on the pull request will provide a place for design discussion, and committing to that branch will enable iterative collaboration. Make sure to follow the [Documentation Guidelines](Documentation%20Guidelines.md).  
The PR will be accepted once X% of collaborators vote in favor of its completion, and it is approved by an [authorized contributor](https://github.com/Ethical-Commons-Project/EthicalMatch-docs/issues/8)
> #todo the create branch and pull-request actions do not exist. This will need to be done manually for now...  
> #todo Here's a [github app](https://github.com/cncf/gitvote) that might make the voting possible

> [!Tip]
> Describe what the feature should accomplish without over-specifying how it should be implemented.  
> *Well-known design patterns are the exception* 
### Development Status Tracking
Each section must have a status label that indicates the current state of progress. This makes it clear what work needs to be done at a glance. Format it like so:  
```
## Feature Header    ![](https://progress-bar.xyz/35%)
```
- Not Started: ![](https://progress-bar.xyz/0)
- Completed: ![](https://progress-bar.xyz/100)
- Subcomponents Partially Completed: ![](https://progress-bar.xyz/35)


> [!Note]
> While the sentiment here is to maintain the sovereignty of the documentation as the sole source of truth, keeping these updated with every code update is a real pain. If you have an idea how to automate this, weigh in on [the Github issue](https://github.com/EthanGunter/EthicalMatch-docs/issues/2)
### 3. Code Implementation
Use the accepted documentation as a guideline for what your code should do. There may be implementation suggestions in the associated GitHub issue and PR, so if you're looking for an idea on how to start, look there. Otherwise, [our discord](https://discord.gg/P7qfVuqMXz) is a great place to have that conversation!  

  > [!Tip]
  > Step 4 requires updating the documentation with your new code. We recommend updating it as you develop, to save you time and headaches down the road.
### 4. Wrapping up and Status Updates
After your pull request is merged into the product, the corresponding GitHub issue will be closed and the feature will be marked as "Done" in the [Feature Development Project](https://github.com/orgs/Ethical-Commons-Project/projects/2/views/1?query=sort%3Aupdated-desc+is%3Aopen). Now the docs need to be updated to reflect your implementation.  
We're looking for 2 things:
1. Mark your feature's [progress bar](#Development%20Status%20Tracking) as completed in the documentation
1. Add examples or visualizations (e.g., graphs or diagrams) to help contributors understand and use your code

> [!Warning]
> If you do not [link](https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/linking-a-pull-request-to-an-issue) your pull request to the issue you were addressing, the automated processes above will not take place, potentially confusing other contributors 

> [!Tip]
> When you make this final documentation pull request, link it to the pull request for your code from step 4 to help it get accepted faster
