## What is _good_ software architecture?
It means that when you make a change, it's as if the entire program was crafted in anticipation of it. You can solve a task with just a few choice function calls that slot in perfectly, leaving not the slightest ripple on the placid surface of the code.

The first key piece is that _architecture is about change_. The measure of a design is how easily it accomodates changes.


### How do you make a change?

Before you can change the code to add a new feature, to fix a bug, or for whatever reason caused you to fire up your editor, you have to understand what the existing code is doing. 

Once you understand the problem and the parts of the code it touches, the actual coding is sometimes trivial.

In short, the flow chart for programming is something like:
![[Pasted image 20260823134806.png]]

## How can decoupling help?
You can define "decoupling" a bunch of ways, but I think if two pieces of code are coupled, it means you can't understand one without understanding the other. If you _de-couple_ them, you can reason about either side independently.

This is a key goal of software architecture: **minimize the amount of knowledge you need to have in-cranium before you can make progress.**

Another definition of decoupling is that a _change_ to one piece of code doesn't necessitate a change to another. We obviously need to change _something_, but the less coupling we have, the less that change ripples throughout the rest of the game.

## At what cost?

Good architecture makes a _huge_ difference in productivity. But, like all things in life, it doesn't come free. Good architecture takes real effort and discipline. Every time you make a change or implement a feature, you have to work hard to integrate it gracefully into the rest of the program. You have to take great care to both organize the code well and _keep_ it organized throughout the thousands of little changes that make up a development cycle.

You have to think about which parts of the program should be decoupled and introduce abstractions at those points. Likewise, you have to determine where extensibility should be engineered in so future changes are easier to make.

Whenever you add a layer of abstraction or a place where extensibility is supported, you're _speculating_ that you will need that flexibility later. You're adding code and complexity to your game that takes time to develop, debug, and maintain.

"Some folks coined the term 'YAGNI' -- **You aren't gonna need it** -- as a mantra to use to fight this urge to speculate about what your future self may want."

## Performance and Speed

A lot of software architecture is about making your program more flexible. It's about making it take less effort to change it. 

But performance is all about assumptions. The practice of optimization thrives on concrete limitations.

The faster you can try out ideas and see how they feel, the more you can try and the more likely you are to find something great. Even after you've found the right mechanics, you need plenty of time for tuning.

There is no easy answer here. Making your program more flexible so you can prototype faster will have some performance cost. Likewise, optimizing your code will make it less flexible.

It's easier to make a fun game fast than it is to make a fast game fun.

## The Good in Bad Code

Writing well-architected code takes careful thought, and that translates to time. Moreso, _maintaining_ a good architecture over the life of a project takes a lot of effort.

This is good when you're going to be living in and working on that code for a long time. But game design requires a lot of experimentation and exploration. Especially early on, it's common to write code that you know you'll throw away.

If you just want to find out if some gameplay idea plays right at all, architecting it beautifully means burning more time before you actually get it on screen and get some feedback. If it ends up not working, that time spent making the code elegant goes to waste when you delete it.

Prototyping -- slapping together code that's just barely functional enough to answer a design question -- is a perfectly legitimate programming practice. There is a very large caveat, though. If you write throwaway code, you _must_ ensure you're able to throw it away.

## Striking a Balance

1. We want nice architecture so the code is easier to understand over the lifetime of the project.
2. We want fast runtime performance.
3. We want to get today's features done quickly.

These goals are at least partially in opposition. Good architecture improves productivity over the long term, but maintaining it means every change requires a little more effort to keep things clean.

There is no simple answer here, just trade-offs. 

## Simplicity

if there is any method that eases these constraints, it's _simplicity_. Simple code doesn't necessarily takes less time to _write_. A good solution isn't an accretion of code, it's a _distillation_ of it.

When we think of elefant solutions, what we often have in mind is a _general_ one: A small bit of logic that still correctly covers a large space of use cases.


* Abstraction and decoupling make evolving your program faster and easier, but don't waste time doing them unless you're confident the code in question needs that flexibility.
* Think about and design for performance throughout your development cycle, but put off the low-level, nitty-gritty optimizations that lock assumptions into your code until as late as possible.
* Move quickly to explore your game's design space, but don't go as fast that you leave a mess behind you. You'll have to live with it, after all.
* If you're going to ditch code, don't waste time making it pretty. Rock stars trash hotel rooms because they know they're going to check out the next day.
* But, most of all, **if you want to make something fun, have fun making it.**

