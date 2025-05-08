### Principles:

- SRP (Single Responsibility Principle)
- OCP (Open Closed Principle)

### Miscellaneous Learnings:

#### ch-3 (functions)
- names of functions/variables should tell me everything
- functions should do one thing and they should do it well
- functions should have a constant level of abstraction, they should not be mixed like low level .append and high level like getHTML()
- functions should be max 20 lines long
- functions should have no side-effects (function promises to do one thing, but it also does other hidden things)


### Principal explanatoins: 

#### SRP:
    One reason to change:
    If a class has multiple responsibilities, it might need to be modified for reasons unrelated to its core purpose, leading to a more complex and difficult-to-maintain codebase. 

#### OCP:
    Open for extension:
    You should be able to add new features or behaviors to a class without changing its original source code. 
    Closed for modification:
    Once a class is written and tested, it should not be modified to add new features, but rather extended through inheritance or composition. 
