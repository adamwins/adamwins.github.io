---
layout: essay
type: essay
title: "Think Before You Code"
# All dates must be YYYY-MM-DD format!
date: 2024-04-25
published: true
labels:
  - Design Patterns
  - Software Engineering
---

<img width="400px" class="rounded float-start pe-4" src="../img/cotton/design_patterns.png">

## Everyone Needs a Plan

We’ve all been at that starting point in our software engineering journey, where we are unsure of what we’re doing and just typing lines of code into our IDE and praying that our application works correctly. At some point, though, we all realize that if we take the time to think about an approach to our code and structure it in certain ways, we can more effectively solve problems. As we mature throughout our software engineering journey, we get better at recognizing when to apply these patterns to problems, and as such these patterns become reusable. These patterns are known as design patterns, and they help a lot in structuring your application and finding solutions to problems that share similarities.


## Reduce, Reuse, Recycle

If I were to compare design patterns, which are a more abstract approach to solving problems, in terms of actual code, they serve a similar purpose as react components. Although not quite the same, react components can be reused and applied whenever applicable. Design patterns, just like functions, algorithms, and methods in programming, reduce a complex idea into a simple pattern, reuse the pattern in similar applications, and recycle patterns when necessary.

## How Does This Apply to Me?
One example of a design pattern I implemented was the singleton pattern, which was the same one used in the example Bowfolio template. The singleton design pattern ensures that a class has only one instance and provides a global point of access to that instance. For example, in our implementation, we leveraged the singleton pattern to create a centralized logging system. By encapsulating the logging functionality within a singleton class, we guarantee that all parts of the application share the same logger instance. This not only promotes consistency in logging behavior but also enhances performance by avoiding unnecessary overhead associated with creating multiple logger objects."

Note- ChatGpt was used to correct any grammar and punctuation mistakes as well as elaborate on the singleton pattern.
