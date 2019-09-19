# Evaluating a take-home exercise

There are two stages to screening a take-home exercise solution:

* An initial, quick score which the solution will have to pass before moving onto the second stage
* A pair of engineers spend a couple of hours reviewing the solution in detail

Note that meeting the cut-off score is a "necessary but not sufficient" condition to consider a candidate for the in-person interview. If a solution passes the cut-off score, then a pair of engineers will review the exercise more thoroughly and decide on whether we should bring a candidate in for the in-person interview or not. 

If it doesn't, the solution is rejected and we **must** respond with an appropriate rejection mail.

## Quick Score

The scoring has four different sections \(see table below\), all of which contribute a certain number of points to the overall score of a solution. The scoring process has been designed to compensate for a solution lacking in one aspect, but done well in others

1. For each of the four sections in the table below, look at the state of the repository and select an appropriate score for the role the candidate is applying for.
2. Sum up the scores for the individual sections \(Documentation, Commit History, Testing, and Application\).
3. If the total score is greater than or equal to the cut-off score for a role, then proceed with the detailed evaluation of the exercise.

| Criteria | P2 \(2 - 4 years\) | P3 \(4 - 8 years\) |
| :--- | :--- | :--- |
| **Documentation** |  |  |
| No documentation in the repository | 0 | -1 |
| Some documentation with basic setup instructions or feature descriptions | 1 | 1 |
| Detailed documentation with setup, screenshots, configuration instructions, etc | 2 | 2 |
| **Commit History \(See** [**Note 1**](scoring-a-take-home-exercise.md#note-1) **below\)** |  |  |
| The repository has a few large commits \(Exceptions are commits with auto-generated code like Room schemas or the initial commit when initialising a project through an IDE or a CLI\) | 0 | -1 |
| The repository has some small-ish commits with clear \(what the commit does\) messages | 1 | 1 |
| The repository has many tiny, atomic commits with clear, descriptive \(what the commit does and why, when appropriate\) messages | 2 | 2 |
| **Testing** |  |  |
| There are either no tests, or a few tests that aren't really that useful | 0 | -1 |
| Tests for business logic are present, but they are tested via instrumentation/UI tests | 1 | 1 |
| Business logic is tested using a good number of unit tests, and there might be instrumented/UI tests for testing platform integration | 2 | 2 |
| **Application** |  |  |
| Barebones, developer UI with no error/touch feedback to the user | 0 | -1 |
| Functional UI, and with error feedback and/or touch feedback | 1 | 1 |
| Polished UI, with thought put into the user experience and/or with nice transitions and animations | 2 | 2 |
|  |  |  |
| **Minimum Score Required** | **4** | **5** |

## Pair Review

> TO BE DONE

## Notes

#### Note 1

The ideal "size" of a commit diff is subjective. A good rule of thumb would be to follow the section on ["Small CLs"](https://google.github.io/eng-practices/review/developer/small-cls.html) in the Google Engineering Practices guide.

## Recommended Reading and watching

* Google's guide for Change List authors: [https://google.github.io/eng-practices/review/developer/](https://google.github.io/eng-practices/review/developer/)
* Write awesome tests by Jeroen Mols: [https://www.youtube.com/watch?v=F8Gc8Nwf0yk](https://www.youtube.com/watch?v=F8Gc8Nwf0yk)



