# A first example
## Writing test suite before you do refactoring
Before starting refactor your code, please make sure you have a solid set of tests for that section of code. Normally refactoring means introducing huge amount of changes to your code, during this process you may make some mistakes no matter how careful you are. With testing along this process, you can make sure your refactor doesn't break the code's outer behavior.

## Step by step
Break your refactoring into several small steps. Make a small change at a time, after the change, run the test cases you prepared to make sure your code still works as expected. With a large amount of changes, it will be difficult for you to debug when things fuck up.
> It's an important habit to test after every refactoring, however simple. Mistakes are easy to make - at least,, I find them easy to make. **Testing after each change means that when I make a mistake, I only have a small change to consider in order to spot the error, which makes it far easier to find and fix**.

## Make use of git commit
Do a git commit after a small refactoring is a good practice. With a small commit at a time, you can easily rollback to previous commit, and replay all your changes to spot the error.

Squash all of the commit into a single one after your refactoring.

## Variable naming
> Always name the return value from a function "result".

For a dynamic language like Javascript, it is encouraged to name its function parameter with its type. For example, classArr, etc.

> **Good code should clearly convey what it is doing, and variable names are a key to clear code.**
```
bad: res
good: result

bad: fById
good: findById
```

## Structure brings performance issue
Most of time refactoring brings performance slow-downs to your system temporarily, you should ignore it first and only focus on the refactoring. After the refactoring, you can start to do performance tuning.

It's more important to maintain the clarity of your code than the brevity.
> Brevity is the soul of wit, but clarity is the soul of evolvable software.

## What is good code
> I'm talking about improving the code - but programmers love to argue about what good code looks like. I know some people object to my preference for small, well-named functions. If we consider this to be a matter of aesthetics, where nothing is either good or bad but thinking makes it so, we lack any guide but personal taste. I believe, however that we can go beyond taste and say that **the true test of good code is how easy it is to change it.** Code should be obvious: When someone needs to make the change,they should be able to find the code to be changed easily and to make the change quickly without introducing any errors.