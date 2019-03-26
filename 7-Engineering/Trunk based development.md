# WIP: Trunk-based Development

> ### A source-control branching model, where developers collaborate on code in a single branch called `master` (or “trunk”), and resist any pressure to create other long-lived development branches. They therefore avoid merge hell, do not break the build, and live happily ever after.
> _From [TrunkBasedDevelopment.com](https://trunkbaseddevelopment.com/)_

TBD promotes short-lived feature branches and frequent merges with the trunk. A branch usually has only one developer, it doesn’t last more than a day or two, flows through CI and code review, and finally gets merged into `master`.

TBD is a key enabler of  Continuous Integration and by extension  Continuous Deployment. When individuals on a team are committing changes to `master` multiple times a day, it becomes easy to satisfy the core requirement of Continuous Integration that all team members commit to trunk at least once every 24 hours. 

This ensures the codebase is always releasable on demand and helps to make Continuous Delivery a reality. This also means that TBD is the opposite of models like Git Flow, where features are developed in parallel to `master`, living in long-running branches. 

> ### Branches create distance between developers and we do not want that
> _Frank Compagner, Guerrilla Games_ 

There are two ways that TBD is accomplished:

  1. In large companies which have developer experience teams (like Google), everyone commits directly to the `master` branch. The commits do not become part of the repository immediately -- they're usually held in a staging server, where code review happens, and CI tools are run. Once everything looks good, the commits are applied to `master` and become visible to the rest of the team.
  
  1. Smaller teams (like ours) can accomplish the same thing by using Pull Requests. We create short-lived daily branches and raise a PR, usually at the end of the work day. The PR is used for build checking (CI), and it allow developers to engage in eager and continuous code review. This probably raises many questions in your head, so read on!
  
## Daily branches

To ensure that constant integration of code is happening, we prefer making "daily branches". This doesn't strictly mean a branch every day, but branches _rarely last beyond 2 days_ without being raised as a PR. We also ensure that the changeset of a PR doesn't exceed _300-400 lines of code_.

### Conventions

  - Daily branches are named as `initials/date/subject`
  - For example, if your initials are PK, and you raise a branch on 17th December to update the Android Gradle Plugin, your branch title should be something like `pk/17dec/upgrade-agp`
  - No underscores allowed, only dashes

## Releases 

  - release branches 
  - cherry picking from master 
  

## Associated techniques 

  - branch by abstraction
  - feature flags 
