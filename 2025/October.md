# October 2025

# Week of Oct. 20

- How to deal with ambiguous, large systems (especially when making changes or refactoring)
  - Make the system observable: document inputs, outputs, entrypoints, integrations, etc.
  - Start with a diagram of how the system works (data flows, work flows, etc.)
    - Doesn't matter if you don't know things _yet_ --- it's all about knowledge + context building
  - Log unknowns so they can be revisited
  - Codify any assumptions (i.e., put them in code-level comments, etc.) -> brings assumptions to light and minimizes _wrong_ assumptions
  - If you're learning a new system, work in notebooks or some sort of scratch code
    - Once you understand the problem and your changes, then you can start making quality code
    - Quality doesn't yet matter if you're learning --- only if you're deploying it already
    - This reduces the need to "clean up"
  - When you're making changes, add lightweight tests or assertions -> this makes the system self-validating and reveals where breakages are happening
- When working on changes (small or large):
  - Always have a working baseline to start from
    - Run everything locally so that you know things work before you even try to have others review it
    - DevEx helps here
    - Don't build everything all at once --- make small changes that slowly build up the baseline
