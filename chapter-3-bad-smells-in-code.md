# Bad smells in code
## Mysterious Name
One of the most important parts of clear code is good names, so we put a lot of thought into naming functions, modules, variables, classes, so they clearly communicate what they do and how to use them.

When you can think of a good name for something, it's often a sign of a deeper malaise.

## Long Function
Since the early days of programming, people have realized that the longer a function is, the more difficult it is to understand.

The real key to making it easy to understand small functions is good naming. If you have a good name for a function, you mostly don't need to look at its body.

A heuristic we follow is that whenever we feel the need to comment something, we write a function instead. Such a function contains the code that we wanted to comment but is named after the intention of the code rather than the way it works.

## Long Parameter List
If you can obtain one parameter by asking another parameter for it, you can use Replace Parameter with Query to remove the second parameter.

## Mutable Data
Changes to data can often lead to unexpected consequences and tricky bugs. I can update some data here, not realizing that another part of the software expects something different and now fails - a failure that's particularly hard to spot if it only happens under rare conditions. For this reason, an entire school of software development - functional programming - is based on the notion that data should never change and that updating a data structure should always return a new copy of the structure with the change, leaving the old data pristine.

## Alternatives Classes with Different Interfaces
One of the great benefits of using classes is the support for substitution, allowing one class to swap in for another in times of need. But this works if their interfaces are the same.