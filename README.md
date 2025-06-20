### Principles:

- SRP (Single Responsibility Principle)
- OCP (Open Closed Principle)
- DRY (Don't Repeat Yourself)

### Miscellaneous Learnings:

#### ch-3 (functions)
- names of functions/variables should tell me everything
- functions should do one thing and they should do it well
- functions should have a constant level of abstraction, they should not be mixed like low level .append and high level like getHTML()
- functions should be max 20 lines long
- ideal no. of arguments for a function is 0(niladic), then one(monadic), followed by two(dyadic), more than them should be avoided
- flag arguments like true/false should be avoided as it clearly hints that the function does more than one thing
- functions should have no side-effects (function promises to do one thing, but it also does other hidden things)
- output arguments should be avoided (addData(s) is ambiguous as it does not tell it's adding data to something else or to s), instead use setters of some class or object
- the getters and the setters should be seperate
- prefer exceptions rather than returning error codes, exceptions can be dealt with in try/catch blocks, while error codes need to be dealt with on the function calls
- the real goal is to tell the story of the system

#### ch-4 (comments)
- comments are used to compensate for our failure to express ourself in code
- some comments although are useful like regex code examples in comment
- providing the intent behind a decision which was taken at the time
- warning of consequences, useful and might prevent accidents, eg: warning the coder that the following test case is commented as it takes too long to run
- TODO comments are beneficial : should explain why the function has a degenerate implementation and what that function's future should be
- leaving a commented out code should be strictly avoided

#### ch-5 (formatting)
- if one function calls another, they should be vertically close and the caller should be above the callee

#### ch-6 (objects and data structures)
- objects do not expose data but just the functions/behaviour, so it is easy to add new data but difficult to add new behaviour
- data-structures do not have any behaviour, they just expose data, so it is easy to add new behaviour/methods but hard to add new data as all functions must change

### Principal explanations: 

#### SRP:
    One reason to change:
    If a class has multiple responsibilities, it might need to be modified for reasons unrelated to its core purpose, leading to a more complex and difficult-to-maintain codebase. 

#### OCP:
    Open for extension:
    You should be able to add new features or behaviors to a class without changing its original source code. 
    Closed for modification:
    Once a class is written and tested, it should not be modified to add new features, but rather extended through inheritance or composition. 
