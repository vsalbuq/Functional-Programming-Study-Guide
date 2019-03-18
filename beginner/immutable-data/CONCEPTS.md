# IMMUTABLE DATA
## What's the value of _x_?

Imagine for a moment that I'm an algebra teacher. You are a student in my class. I write down on the board:

```
x = 2 + 2
x = ?
```
You probably would say "Four!", without thinking too much about it. But I would say "Wrong! It's one!".

How would you feel about that? You would surely want an answer to why and how it would be possible. I would say: "Well... Before you answered, some other person had access to `x` and used it to do calculate `x = 2 - 1`".

This is insane. But let's think about what is wrong in this little story. Spoiler alert: It's related to the mistake of using algebra as we do ~~(imperative)~~ programming.

## Equality vs. Assignment
In algebra, the equality sign (`=`) represents comparison, not assignment. So, `x = 2 + 2` just says _"the value of `x` since the begining of this equation **always** have been four"_.

When you look at programming, if something can be changed where you are not looking (or have no access), it makes it difficult to predict what your code will do. It is one thing to do simple code, like a calculator or some minimal script with nothing more than a few lines. But when your code begins to grow, things begin to work like that story, especially if you have shared that `x` variable with all the parts of the code. It's easy to get unexpected behavior, because everyone is changing `x` at runtime, when your code is running.

Conclusion: **It is easier to reason about your code when you use immutable data.**

## So... How can I apply this concept on JavaScript code?
~~write here~~


## Conclusion
It is reasonable that 50 years ago people had to be extremely careful concerning the amount of space while storing data. But our storage technology has grown so much since then that companies around the world are literaly storing anything they can (big data). There were restrictive laws they should use to program at that time that are not true anymore.

Imagine if you had to build a car a thousand times bigger. Probably the laws you would obey to build that would be far different from the ones people use now to build regular cars. This is the proportion of change we are talking about. Storage technology is far different from 50 years ago, but we still using those restrictions.

If performance is not going to be changed significantly, you should focus on what would make your code more readable and predictable to human brains.
