# EOVE's organisation-wise configuration files

## Creating a new issue

Pick an existing template when possible:

- "Eove bug issue" to report a bug/regression concerning end-user
    - criticity will be evaluated in template
    - production code only
- "Eove feature/enhancement issue" to describe a feature/enhancement for eove products
    - could be a brand new feature
    - could be a change to an existing feature
    - should concern end-user
- "Eove technical issue" to describe a technical modification (build, tests, refactoring)
    - could be a dependency update
    - when you add more tests out of a feature
    - when you modify the build

## Labelling the issue

When issue is created, the template may have applied a label automatically.

If label is missing, pick one among the following list:

- `bug:critical`: A bug with an accepted risk
- `bug:minor`: A bug with no risk for the patient
- `bug:nc`: A bug with an unacceptable risk
- `documentation`: Improvements or additions to documentation
- `feature`: A new feature or a change to an existing one
- `technical`: Far from end-user (refactoring, build, tests)

The exhaustive list is available
at [Repository labels](https://github.com/organizations/eove/settings/repository-defaults).
