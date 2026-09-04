# Pragmatic Programmer

Book by David Thomas and Andrew Hunt

This is the JavaScript edition

## Key

❓: unresolved questions
🗨: my own thoughts

## Table of Content

- [Pragmatic Programmer](#pragmatic-programmer)
  - [Key](#key)
  - [Table of Content](#table-of-content)
  - [Introduction](#introduction)
  - [Chapter 1: A Pragmatic Philosophy](#chapter-1-a-pragmatic-philosophy)
    - [1. It's Your Life](#1-its-your-life)
    - [2. The Cat Ate My Source Code](#2-the-cat-ate-my-source-code)
    - [3. Software Entropy](#3-software-entropy)
    - [4. Stone Soup and Boiled Frogs](#4-stone-soup-and-boiled-frogs)
    - [5. Good-Enough Software](#5-good-enough-software)
    - [6. Your Knowledge Portfolio](#6-your-knowledge-portfolio)
    - [7. Communicate](#7-communicate)
  - [Chapter 2: A Pragmatic Approach](#chapter-2-a-pragmatic-approach)
    - [8. The Essence of Good Design](#8-the-essence-of-good-design)
    - [9. DRY - The Evils of Duplication](#9-dry---the-evils-of-duplication)
    - [10. Orthogonality](#10-orthogonality)
    - [11. Reversibility](#11-reversibility)
    - [12. Tracer Bullets](#12-tracer-bullets)
    - [13. Prototypes and Post-it Notes](#13-prototypes-and-post-it-notes)
    - [14. Domain Languages](#14-domain-languages)
    - [15. Estimating](#15-estimating)
  - [Chapter 3: The Basic Tools](#chapter-3-the-basic-tools)
    - [16. The Power of Plain Text](#16-the-power-of-plain-text)
    - [17. Shell Games](#17-shell-games)
    - [18. Power Editing](#18-power-editing)
    - [19. Version Control](#19-version-control)
    - [20. Debugging](#20-debugging)
    - [21. Text Manipulation](#21-text-manipulation)
    - [22. Engineering Daybooks](#22-engineering-daybooks)
  - [Chapter 4: Pragmatic Paranoia](#chapter-4-pragmatic-paranoia)
    - [23. Design by Contract](#23-design-by-contract)
    - [24. Dead Programs Tell No Lies](#24-dead-programs-tell-no-lies)
    - [25. Assertive Programming](#25-assertive-programming)
    - [26. How to Balance Resources](#26-how-to-balance-resources)
    - [27. Don't Outrun Your Headlights](#27-dont-outrun-your-headlights)
  - [Chapter 5: Bend, or Break](#chapter-5-bend-or-break)
    - [28. Decoupling](#28-decoupling)
    - [29. Juggling the Real World](#29-juggling-the-real-world)
    - [30. Transforming Programming](#30-transforming-programming)
    - [31. Inheritance Tax](#31-inheritance-tax)
    - [32. Configuration](#32-configuration)
  - [Chapter 6: Concurrency](#chapter-6-concurrency)
    - [33. Breaking Temporal Coupling](#33-breaking-temporal-coupling)
    - [34. Shared State Is Incorrect State](#34-shared-state-is-incorrect-state)
    - [35. Actors and Process](#35-actors-and-process)
    - [36. Blackboards](#36-blackboards)
    - [Chapter 7. While You Are Coding](#chapter-7-while-you-are-coding)
    - [37. Listen to Your Lizard Brain](#37-listen-to-your-lizard-brain)
    - [38. Programming by Coincidence](#38-programming-by-coincidence)
    - [39. Algorithm Speed](#39-algorithm-speed)
    - [40. Refactoring](#40-refactoring)
    - [41. Test to Code](#41-test-to-code)
    - [42. Property-Based Testing](#42-property-based-testing)
    - [43. Stay Safe Out There](#43-stay-safe-out-there)
    - [44. Naming Things](#44-naming-things)
  - [Chapter 8. Before the Project](#chapter-8-before-the-project)
    - [45. The Requirements Pit](#45-the-requirements-pit)
    - [46. Solving Impossible Puzzle](#46-solving-impossible-puzzle)
    - [47. Working Together](#47-working-together)
    - [48. The Essence of Agility](#48-the-essence-of-agility)
  - [Chapter 9: Pragmatic Projects](#chapter-9-pragmatic-projects)
    - [49. Pragmatic Teams](#49-pragmatic-teams)
    - [50. Coconuts Don't Cut It](#50-coconuts-dont-cut-it)
    - [51. Pragmatic Started Kit](#51-pragmatic-started-kit)
    - [52. Delight Your Users](#52-delight-your-users)
    - [53. Pride and Prejudice](#53-pride-and-prejudice)
  - [Footnotes](#footnotes)

## Introduction

> Programming is about making the future less painful – Saron Yitbarek

🗨 And it's not what you might think :D
🗨 Programming is about making your future, and the future of programmers who will touch your code later: less painful. That's what good software engineering is about.
🗨 It reminds me of a presentation by Matthias Felleisen about what he calls Social Responsibility of a Programmer. I expected it to be about our role in society, "We have the responsibility to bring society forward!", "we shape the future", no no no... nothing of that sort. From his point of view software developement is a _social debt_ towards developers who will maintain the code after you. It could be you some years later or "someone who isn't even born yet". I think that even thought it's not complete, it is a fresh and humble prespective and doesn't glorify the field. Yes it _is_ challenging work, but as someone one described it: "it's not an act of heroism". We often fall into this idea of being a [genius programmer](https://youtu.be/0SARbwvhupQ?si=aNbnef-WN5Kh7IQA) or something when we are simply part of the service sector, we're not too different from plumbers, carpenters, or doctors; while of course while having some unique properties. But we're just offering a service, we are not like philosophers, policy makers, intellectuals and thinkers who change people's lives and beliefs about the world. and this does not mean we don't have ethical responsbility or that the job is worthless. And well, I truly love this field so much. That's why I'm reading this book anyway. But once I understood this idea I felt humbled.

🗨 I was reading the introduction of Clean Code, which I plan to read after this book.
In the introduction the author says:

> You and I, we programmers, rule the world. Other people think they rule the world, but then they hand the rules to us, and _we_ write those rules — the software.

🗨 And to be fair, just after that Robert Martin explained how can bad software damage society and even kill people, and we must learn how to become professionals. But that line really made me uncomfortable honestly.

🗨 The book quickly mentions the issue of terminology, which I really enjoy

> Either perfectly good English words that have been corrupted to mean something technical, or horrendous made-up words that have been assigned meanings by computer scientists with a grudge against the language

🗨 I'm not that attached to English as it's not my first language, but some terms really make you feel whoever came up with them really hated language. _Memoization_ immediately comes to mind.

> This book will help you become a better programmer.

🗨 The book is called Pragmatic Programmer, and the term pragmatic caught my eye because I know some philosophy. Pragmatism is a philosophy from the 19th century that had a huge impact on the world; it has its unique epistemological basis (e.g., about the nature of knowledge) and many concepts that all revolve around the idea of practicality; knowledge itself is judged by its practicality.

🗨 But when people say someone is pragmatic, they often don't mean the philosophy, but they simply mean the person is practical and gets the job done. So from what I understand, the book has nothing to do about the pragmatic philosophy at all; it's about the practical wisdom of two experienced programmers - though it's important to note that our philosophies and our values inevitably will affect our thoughts and our ink.

> Tip 1: Care About Your Craft

🗨 The book's cover displays some carpenter's tools; this is related to the idea of craftsmanship and seeing your job as a craft you seek to master. Some people like this idea, and others would tell them to stop fantasizing! You're just a cog in the wheel. I think there is some middle ground. And I think it's also freeing to start treating it as a craft; it's not even about the joy you get, which is real, but realizing it's just a service sector; it's the same for doctors, carpenters, plumbers, etc. We're just offering a service that people need; it's not some heroic act to build software.

> Tip 2: Think About Your Work

🗨 It's important to think about your work, and this reminds me of one quote by Dijkstra's that I heard in Remzi's operating systems online lectures. Dijkstra explains that experience is not the same as wisdom; to have wisdom, you need both experience and reflection. Constantly reflecting on your work, and more importantly, on yourself, your emotions, is a great path for growth. And it's not easy because most of us are very distant from ourselves and our thoughts.
🗨 When it comes to programming, I like to call it deliberate thinking; it's something I learned as a CS student by seeing it in different contexts and realizing its importance.
I've seen that even experienced developers do this. For example I've used to watch Ali Fadel, a software engineer who worked at Amazon, and made videos on competitive programming in Arabic.
One thing I kept noticing: he would explain a solution, and then pause and say 'now, why is that correct' or 'why is that not correct'. That made me reflect; I don't remember asking myself why a solution is not correct!

I have only one method that I recommend extensively—it's called think before you write. – Richard Hamming

'Think first, experiment later.'[^think] – CS2510

🗨 I remember now how in High School I used to find it odd that, unlike English essays, when writing French essays where we must start by explicitly writing the problématique, i.e., the problem we are discussing, I didn't realize then that it had some pedagogical reasons.

🗨The Book also points to an important thing, which is 'think about your work while you're doing it'. We often think we think 'We'll think about it later, I'll reflect later', but there are many things that could distract us, it's better to use every opportunity to reflect, and this a know fact in good learning which is to learn actively, instead of underlining or highlighting the book you're reading stop for a moment and try to recall the point the writer is making using your own words, try to think about it and critique it

## Chapter 1: A Pragmatic Philosophy

### 1. It's Your Life

> Tip 3: You Have Agency

🗨 The book starts with some motivational speech - but it's not that annoying; it seems just some useful and pragmatic (= practical) tips the authors have learned over the years.

The authors have noticed that many programmers are very concerned and maybe feeling uncomfortable at their jobs or life, but they are doing nothing, even though this field is one of the best fields when it comes to agency; there are a million things you can do!

### 2. The Cat Ate My Source Code

Take responsibility for your mistakes and shortcomings.
It's not a fun thing to happen; it's not easy to admit mistakes, but in my opinion, I think it's honorable.
The book also explains that the team should be able to rely on and trust you. And that trust is built through action; a good team is a team built on trust and interdependence.

🗨 This, for some reason remind of the famous scene you see in too many films, (It's not your fault). As if being mistaken is something to be ashamed of. To me, a good friend or teammate is someone who'd tell you, 'Dude, you messed up! but it's okay, let's find a solution'.
🗨 I understand the culture we're starting to have, the culture of not naming things what they are. It's comforting, and there is nothing wrong with seeking comfort; we all do want that. But I think it's leading us to even worse environments.

> Tip 4: Provide Options, Don't Make Lame Excuses

The section ends with a very practical tip: instead of offering lame excuses when something goes wrong, explain what can be done and offer different options.
Another pro tip: don't just say 'I don't know'; follow it up with 'I'll figure it out'

### 3. Software Entropy

- 🗨 Entropy here is the thermodynamic entropy and not Shannon's Entropy (Information Theory)
- Entropy in thermodynamics is a 'measure of disorder'. And by the laws of physics, any system tends toward the maximum entropy, that is, it tends towards disorder.
- When the software is chaos The author calls it a 'software rot'; they don't seem to be fond of the more optimistic term 'technical debt', because it implies the 'debt' will be paid back, but it often isn't the case.

> Tip 5. Don't Live with Broken Windows

- A broken window in a building is all it takes to instill a feeling that the building is neglected and slowly drives a feeling of hopelessness, and slowly the building will get worse and worse.
- Same goes for software (and many things in life): you should fix problems as soon as you find them, don't let them rot, at the very least show some effort, show that you care. Open an issue for the problem, add some stub 'not implemented yet' message, have a plan to refactor[todo: link to refactor section later] bad code, etc.
- The book claims that such small things, with enough time, are one of the reasons that could ruin even the biggest of projects. The effect of neglect compounds and changes how everyone feels about the project.
- 🗨 I've read that 'Broken Windows Theory' has not been proved yet and there are some discussions about it. But I like the advice, and I think it's valid. It's never a good idea to leave many 'open files' in the background. It's like having monsters lurking in the back of your mind!

TODO: examples

### 4. Stone Soup and Boiled Frogs

Sometimes you know what the right thing to do is, something that will certainly benefit the project, but you'll have to ask for permissions, and it's not easy to convince others, or it takes too much time. The book recommends that in such case you should think of the simplest thing you can ask for and you won't get rejected, after that it's okay to try whetting others' appetite by showing them a 'glimpse of the future', basically saying 'Of course it would be nicer if we add add this or that feature', but pretend it's not that important and wait, there is a good change they would tell you to implement it.

🗨 This is a general social skill I someone taught me, that is, not trying too hard to offer what you have if the other part doesn't seem to care, like when you want to advise someone who doesn't seem to care, sometimes talking too much doesn't help and makes your words less meaningful, this is clearly true for school teachers for instance, the teacher's words might lose impact if they repeat it too many times. Sometimes silence could intrigue the student because it's different and makes them want to hear from you.

> Tip 6: Be a Catalyst for Change

The book brings up the famous Boiled Frogs story, that if you throw a frog in some hot water, it will jump immediately, but if you gradually heat the water, it won't notice. That's not what happens in real life, but it's the moral of the story is worth noting.

> Tip 7: Remember the Big Picture

You need to know what's going on around you in the project and in life in general. You need to understand the big picture.
The book even recommends that you develop situational awareness and observation skills; for instance, close your eyes. - well you can't read like that - but try to count the number of light bulbs in the room you're in, the number of people in the room, etc. It's a good idea to develop this skill and sharpen your mind for details, and do the same for your projects.

### 5. Good-Enough Software

You should know what the minimum quality required for the project, you can spend a lot of time perfecting parts of the system, but don't overdo it. It depends on the kind of software you're working on, but in most cases, releasing 'good enough' software
But you need to define what's 'good enough' for your project; it surely doesn't mean low-quality code and neglecting important things like security.

> Tip 8: Make Quality a Requirements Issue

### 6. Your Knowledge Portfolio

- Tech changes a lot, and you need a strategy for coping.
- Your knowledge portfolio encompasses many things, including all of your experiences, domain knowledge, CS knowledge, etc.
- You should invest in your knowledge portfolio.
  The hard part is forming a habit of learning and expanding your knowledge portfolio. But it's very rewarding as you'll be learning so much without even thinking about it.
- You should create a habit, even if you do a little bit every day, because what matters more in the long term is the habit you're building, not what you're learning.
- Variety matters; the more different the things you know, the better. You certainly must master at least one technology, but you should absolutely learn different technologies.
- It's risky but very rewarding to learn an emerging technology.

> Tip 9: Invest Regularly in Your Knowledge Portfolio

Some nice goals to set

- Learn at least one new language every year.
- Read a technical book each month.
- Read nontechnical books, too! Human beings are cool too!
- Take classes at some local or online college or university.

🗨 I have taken a lot of online courses in the past three years; there are a few courses that I highly recommend: Learning How to Learn, Programming Languages

- Participate in local user groups and meetups.

Isolation can be deadly to your career;

🗨 I think it's really interesting that everyone gives this advice; everyone experienced in this field keeps giving this same advice.

- Experiment with different environments
  - try Linux if you've been using Windows
    - 🗨 don't do the opposite thing
  - try some new IDE if you're used to just makefiles, etc.
- Stay current: read news about what's happening, even on technologies you don't typically use.
  - 🗨 I like going through Hacker News, it made me realize you don't really need to use social media (and potentially waste time) to hear about what's happening
  - 🗨 I like this channel, 'The PrimeTime'; the man's content is really fun, and it's really short and gives you an idea of what's happening.
- Keep learning and expanding your knowledge; it's okay if you learn something (e.g., some language), but you don't really end up using it at work; the act of learning itself gives you richer knowledge.
- The book has a neat example: write FP, and you'll write OOP code differently.
- Critical Thinking is extremely important; make sure the accuracy of the knowledge in your portfolio is accurate. Media and hype can create inaccuracies.
- Critical thinking is a skill to develop. Read more about it.
  - Who does this benefit? Sadly, this is a very useful question to think about when hearing a claim

Tip 10: Critically Analyze What You Read and Hear

### 7. Communicate

Tip 11: English is Just Another Programming Language

i.e. you got to master it too!

The book is basically saying, you're going to work with people, so it's important that you learn some communication skills (so-called 'soft skills' that are actually hard to learn)

🗨 Did the book just mention Neuro Linguistic Programming ?! It's a known pseudoscientific approach for communication skills and psychotherapy. The advice in this section is turning into self-help stuff.

The book gives some communication tips that feel generic but do not mean it's devoid of some truth in them: know your audience, know what you want to say, involve the audience, be a listener, make documents look good, and so on…

🗨 Speaking of making documents look good, I've been using Typst for the last year, and it's been great. I like it more than LaTeX[^latex]; it's great for writing pretty much all types of documents.

> Tip 12: It's Both What You Say and The Way You Say It

> Tip 13: Build Documentation, Don't Bolt It On

- Don't add documentation as an afterthought; it should be part of your workflow.
- Add comments to modules and exported functions to help the other devs understand how to use them.
- You don't have to add comments to every single function; that would make things harder to maintain because now you have to modify code and make sure the comments are consistent. Focus on commenting the API[^api], i.e., things other devs will use. For other things, explain the why behind your approaches. The code already explains how it's done.

🗨 I started to noticed I have some undocumented _exported_[^exported] functions.
In JavaScript you can use the JSDoc convention for documentation. It's very useful because IDEs can understands the format. Other programmers could hover over the function name or the params and see hints from the documentation you wrote.

```ts
/**
 * Calculates the total price with tax.
 *
 * @param price - Base price of the item
 * @param taxRate - Tax rate as decimal (0.15 = 15%)
 * @returns Total price including tax
 *
 * @example
 * const total = calculateTotal(100, 0.15); // 115
 */
function calculateTotal(price: number, taxRate: number): number {
  return price * (1 + taxRate);
}
```

![VS code](/media/jsdoc.jpg)

## Chapter 2: A Pragmatic Approach

### 8. The Essence of Good Design

- The word is filled with people eager to shared their software design wisdom. There so many acronyms, patterns, diagrams, architectures, and so on.
- Everything pretty much boils down to a simple idea: ETC

> Tip 14: Good Design Is _Easier to Change_ Than Bad Design

- This is idea is very powerful, as it helps you approach new ideas without feeling intimidated, instead you'd just ask: "Oh cool, how does this help me make software easier to change".
- You can think of any design principle or tips like this.
  - Why is Single Responsibility Principle a good idea?
    - When requirements change, you just need to update one module, i.e. ETC
  - Why is naming important?
    - Good names help you understand, and hence make things easier to change.
- ETC is not a rule, something specific to do, it's a guiding value, a concept that will help you move in the right direction.
- The authors say that you need deliberate practice, constantly asking your self "Did the things I did make the system easier or harder to change?"
- 🗨 Just knowing that the concept exists and that it is important is not enough to actually benefit from it, good practice and time are needed.
- 🗨 As learning scientists often describe it, when you learn something new you're create new neural connections for it. Now you have a _schema_ for the concept ETC. a schema is this set of connected neurons related to something. Now after you learn this concept you can start making connection with other design concepts you know, and that will make the software design schema richer.
- 🗨 With enough practice, you can reach the point where you automatically think about "Is this easier to change" while coding. but at first the initial links are still weak and you probably won't remember to do so. Practice is needed.

- the book recommend adding a reminder whenever you save a file, or maybe after ten times you save a file, I tried it but it was annoying to me.
  - Maybe you could put a sticky note or something in front of you.

- Not always you'll know what to do. Sometiems there are way too many different solutions, you're not sure which one is ETC. Keep it in your notes! make decisions and try to let ETC to guide you, but you might make a mistake, so it's a good idea to take notes in your Engineering Daybook. It's a way to sharpen you instincts and learn from the experience.

🗨 **Assignment**:

- The connection between Functional Programming (FP) vs OOP to being ETC.
  I have learned this idea in Dan Grossman's [Programming Languages](https://www.coursera.org/learn/programming-languages) course
- Let's say you want to create a simple application for geometric operations. Let's say it's some design or drawing software or something.
- You have shapes and you can do operations on them.

| Operation/Shape | Line | Square | Circle |
| --------------- | ---- | ------ | ------ |
| MoveTo          |      |        |        |
| Scale           |      |        |        |
| Rotate          |      |        |        |

In the Object Oriented paradigm we compsoe problems into objects.
So in this problem we will create an class for each kind of data we have and the class contains the methods (operations).

```java
interface Shape {...}
class Line implements Shape {
  void moveTo(x, y) {...}
  void scale(factor) {...}
  void rotate(degree) {...}
}
class Square implements Shape {
  void moveTo(x, y) {...}
  void scale(factor) {...}
  void rotate(degree) {...}
}
class Circle implements Shape {
  void moveTo(x, y) {...}
  void scale(factor) {...}
  void rotate(degree) {...}
}
```

Now to see this you should imagine each class is in a file and maybe you have hundreds of shapes.

1. What happens when you add a new shape in the requirements, let's say a client is complaining your software doesn't have hexagons!

- You would add a new file and write the class Hexagon, you'd implement the Shape interface and make sure the methods are working well. That's it.
- And the nice thing, OOP gives us powerful abstractions because now if you ever wrote a method that takes a shape, you don't need to modify it!

```java
class HelperFunctions {
  void resetPositionToZero(Shape shape) {...}
}
```

you don't need to modify that! it works by default!
This was very Easy to Change.
But hear me out: 2. What happens when the requiments ask for a new _operation_ to be added. Let's say we need to add a setColor operation.
You will have to change every shape class you have and add the method to it, imagine you have hunders of shapes! That's a lot of work! You'd be switching from file to file. It's quite annoying.

TLDR: Easy to add new kinds of data, but harder to add operations.
NB. There are some tricks to deal with this like the Visitor Pattern.

Now let's talk about the Functional Programming approach, it's a pseudo code that looks like TS:

```ts
type Line = { from: number, to: number, ... };
type Square = { topLeftX, topLeftY, ... };
type Circle = { centerX: number, centerY: number, radius: number, ... };
type Shape: Line | Square | Circle
function moveTo(shape: Shape, x, y) {
  switch (shape) {
    case Line: ...
    case Square: ...
    case Circle: ...
  }
}
function scale(shape: Shape, factor) {
  switch (shape) {
    case Line: ...
    case Square: ...
    case Circle: ...
  }
}
function rotate(shape: Shape, degree) {
  switch (shape) {
    case Line: ...
    case Square: ...
    case Circle: ...
  }
}
```

You can imagine that each function will be in a separate module (i.e file) since the functions would grow big and might have many helper functions.

1. what happens if we add a new operation?
   We simple create a new file, and write the new function, it's easy to change and add new functions using this design.
2. what happens if we add a new kind of data?
   sadly, you have to go through every single function you wrote for the for operations and update them (add a new case). Imagine you have hundreds of operations!

🗨 I actually never realized how important software quality was until I went through my first internship, seeing a codebase of thousands of files. If you don't write good code you'll quickly exceed your cognitive load and it's you'll be changing so many files. It's not easy to realize this when you work on small projects.

### 9. DRY - The Evils of Duplication

- As programmers we care about _knowledge_, we document it in spec and implement it. Managing knowledge is part of our job.
- knowledge is constantly changing. you talk to the client or maybe some regulation changes, now suddenly the business logic is outdated.
- Maintenance doesn't start when the project is released, it's part of our daily work as programmers, we're constantly maintaining the code as knowledge and our understanding change day by day.
- It's easy to duplicate knowledge (in spec, code, etc), and it causes a maintenance hell.

> Tip 15. DRY - Don't Repeat Yourself

> Every piece of knowledge must have a single, unambiguous, authoritative representation within a system.

- what's the opposite of that? a single piece of knowledge having two representations. If you change one you need to change the other and that's not ETC.

> It's not a question of whether you'll remember: it's a question of when you'll forget.

- 🗨 Let's star with a simple example of DRY about code duplication. We'll later discuss the bigger picture about DRY, but if you have never heard about DRY before this will give you an idea.

- 🗨 Imagine we have some console app where we print information about items, we often print formatted price in many places.

```ts
function printItemDetails(item) {
  console.log("NAME:")
  console.log(item.name)
  console.log("PRICE:")
  console.log('$' + item.price.toFixed(2))
  ...etc
}
...
function printTotalPrice(items) {
  total = sum(items, item => item.price)
  console.log(`Total: $ ${total.toFixed(2)}`)
  ...etc
}
...
```

🗨 let's say you use that price formatting a hundred time in the project.
Suddenly you realize you want it to use `toFixed(4)`, or maybe you want to update the format based on the locale[^locale] of the user, or anything related to the format. you'd need to go every place you used it and update it! You'd use `grep` or your editor's search and go over all files that include the formatting. That's a pain! That's not DRY code.

🗨 You often hear people saying expressions like "this code is DRY" or "We could do this to make more DRY". Maybe start using it too!

🗨 One solution would be abstracting the formatting into a function:

```ts
function formatPrice(prince) {
  return '$' + price.toFixed(2)
}
function printItemDetails(item) {
  console.log("NAME:")
  console.log(item.name)
  console.log("PRICE:")
  console.log(formatPrice(item.price))
  ...etc
}
...
function printTotalPrice(items) {
  total = sum(items, item => item.price)
  console.log(`Total: ${formatPrice(total)}`)
  ...etc
}
...
```

🗨 This is much more DRY. You could even take a step further and pass the currency as an argument[^arg-vs-param] or use pre-built functions to handle the locale. It's very ETC.

- Common misconception: "DRY is about code duplication"
- _IMPORTANT_: DRY is not _just_ about code duplication (copy pasting code in many places)! it's part of it but DRY is _much more_ than that. The real problem is expressing the same _knowledge_ in many places.
- A bad sign: when you notice a single change in requirements causes you to modify code in many different places. It could mean your code is not DRY.
- IMPORTANT: Not all code duplication is knowledge duplication!

```python
def verify_age(value)
  validate_type(value, int)
  validate_min_integer(value, 0)
...
def verify_quantity(value):
  validate_type(value, int)
  validate_min_integer(value, 0)
```

- Each function represents different knowledge, even though the code is the same, this is _not_ a DRY violation.

🗨 So, from what I understand, each piece of knowledge must map to a single place in code. Otherwise it's not DRY (and hence not ETC).

![DRY diagram](/media/dry.png)

- Be careful about code duplication in comments. You should not comment every single function you create!
- With enough time, the inevitable will happen and code and comments will go out of sync.
- Sometimes you'd find comments that are just re-stating the code logic and the steps done.
- 🗨 It occurred to me that it's as if you're writing the program in two programming languages each time. It's as if you're writing the program in a DSL then writing it again in a programming language!
- 🗨 Here is an example I made up::

```js
/**
 * ROUTE: GET /api/products
 * 1. authenticate user
 *  - otherwise return 401
 * 2. rate limiting: maximum 20 requests per minute
 *  - otherwise return 429
 * 3. verify the user has permissions (products:read)
 *  - otherwise return 403
 * 4. fetch products from database
 * 5. log the request for analytics (products:viewed)
 * 6. return products as JSON
 */
...
const limiter = RateLimiting.ratePerMinute(20)
function GET(request, response) {
  const user = authenticate(request);
  if (!user) return response.status(401).end();
  if (!limiter.check(`view-product:${user.id}`)) {
    return response.status(429).end();
  }

  if (!hasPermission(user, 'products:read')) {
    return response.status(403).end();
  }
  const products = db.products.findAll();
  analytics.track(user.id, 'products:viewed');
  return response.json(products);
}
```

🗨 Now if you change the rate limiting value for instance, you have to remember to update the documentation!

- 🗨 But this made me recall [Peter Norvig](https://github.com/norvig/pytudes)'s "style" (at least from what I understand) and idea of adding a "purpose" to every (or at least, most) functions you write. It's not only for documentation but acts as a problem solving technique because you write the purpose comment _before_ you implement the function. It helps guide your thinking and force you to articulate the intent of the function. This is also explained in the book [How to Design Programs](https://htdp.org/2026-5-28//Book/index.html).

- Here is a simple example from Peter Norvig, also Notice too how the signature (types) also acts as documentation and explain the intent.

```python
def neighbors(cell) -> list[Cell]:
    """All 8 adjacent neighbors of cell."""
    (x, y) = cell
    return [(x-1, y-1), (x, y-1), (x+1, y-1),
            (x-1, y),             (x+1, y),
            (x-1, y+1), (x, y+1), (x+1, y+1)]
```

- So maybe it's fine to have such comments.
- But the gist of the matter: you should not restate what the code does as comments, that's not DRY.
- 🗨 Just noticed, the [table of content](#table-of-content) is certainly a DRY violation, it always keeps going out of sync and I have to update it frequently. So I searched for a solution and found a VS code extention named Markdown All In One that auto updates the TOC.

- DRY violation could also happen in data
  - 🗨 note that when some people use "data" they often mean the data structure, that is, the data representation of the knowledge.

- You should not expose the data structure because then all code that uses it will be coupled with it.

- Here is an example. Let's say I have a configuration module

```js
...
class Configuration {
  static PORT = 3001;
}
export default Configuration;
```

other code might use it.

```js
import config from "../util/config"
...
server.start(config.PORT, () => {console.log("server started...")})
```

Now, if later you wanted to return different port based some environment variable.
you want to return `process.env.PORT` if the `NODE_ENV` is "production", otherwise 3001. And later this could even get more complicated.

```ts
class Configuration {
  static PORT = "??????"; // you could put all the logic here but it will be a mess
}
export default Configuration;
...
```

But now we're stuck, the code that uses PORT is coupled.
That's why it's better to use a method instead. (often called "encapsulation", i.e. using getters and setters)
Now if we change it like this:

```ts
class Configuration {
  static getPORT() {
    return process.env.NODE_ENV === "production" ? process.env.PORT : 3001;
  }
}
export default Configuration;
```

But sadly now you need to go through every function that used to use `config.PORT` and change it to `config.getPORT()`.
This is why it's better to start with such an approach and avoid exposing the internal structure.

By the way it's not true to say the "encapsulation" is an OOP concept. It's actually a general concept in programming. You could for instance use it in functional programming.

```python
def create_point(x, y):
  return (x, y)
def get_x(point):
  return point[0]
def get_y(point):
  return point[1]

def norm(point):
  return sqrt(get_x(point) ** 2 + get_y(point) ** 2)
```

🗨 You could easily now update the data representation of the point (e.g. using a list instead of tuple) and you could update `get_x` and `get_y` without ever needing to update the code that uses them. We say that the code is not _coupled_[^couple].

- ⚠ Some duplication is inevitable, sometimes you export functions, REST APIs, etc. And the users of your APIs need to know some information about, the expected format, paramters, etc. That is a violation of the DRY principle because it is a duplication of knowledge. But it cannot be avoided. Imagine the backend changes the endpoint `POST /api/products` to accept different information about the product, the frontend has to be updated too. But there are ways to cope with it and minimize the pain.
- Duplication Across APIs
  - The book mentions using OpenAPI as a solution
  - it looks amazing, never heard of it before, I also heard many frameworks like nestjs integrates it well. It allows generating API documentation and allows generating the frontend services automatically! #TODO: try this stuff

content to read or watch:

- https://dev.to/senior-debugger/how-we-streamlined-frontend-development-with-openapi-4dn2
- https://www.youtube.com/watch?v=_2-paQxpF7E
- https://www.youtube.com/watch?v=3IKbLDbq5ww&time_continue=393&-embeds_referring_euri=https%3A%2F%2Fwww.google.com%2F
- https://youtu.be/0hx17FfzrKM?si=WVjs8fZC15Rmq2V_

I noticed that the frontend for instance would call the endpoints but it's not if we change the backend endpoint we need to remember to update the frontend endpoint (in the fetch function)

it's interesting, I heard nest uses OpenAPI and it allows for generating the frontend services automatically from the OpenAPI spec. this makes it more DRY.

- [ ] Learn this stuff

- Interdeveloper duplication
- it's really hard to detect
- communication matters here.
  the problem is duplication at a module-level
  sometimes it not clear where some functionality should be implemented, it's not clear under what "area of responsibility" it is. so it gets implemented many times.
- communication is key here.

- assign a team member as the project librarian, who helps the exchange of knowledge. I like this idea.

- A source tree (or source-tree) has two main meanings: a folder hierarchy containing computer program source code

- create a shared place where people add their helpers, etc.
  > Tip 16: Make It Easy to Reuse

all you can do is to try to foster an environment where sharing stuff easier to things don't get duplicated.

> This is not easy, people won't actually do it

Just do your best.

### 10. Orthogonality

- This is one of the topics that's often taught implicitely in other different appraoches and techniques. But it's very useful.
- In math, two vectors like (0, 1) and (1, 0) are orthogonal, whith means they are _independent_.
- A programming _orthogonality_ is some kind of independence or decoupling
  - one a change in one thing doesn't affect a change in another thing
    > Tip 17: Eliminate Effects Between Unrelated Things
- Let's say you created a dekstop GUI for some project, then realized you needed a mobile interface. If the code is orthogonal you should be able to do that easily without updating the backend.
- Components[^component] should be "self-contained", with a single well-defined purpous (often called _cohesion_[^cohesion])
- This helps make the system more ETC, you can change a component's internals without worrying it will affect other components. (As long as you don't change the API)
- There are many benefits for having orthogonal components
  - ETC, it's all about ETC
  - Problems are isolated, they don't propagate a lot in the system, it's easier to fix and replace.
  - Easier to test, reuse, ETC, etc.
    - because you can tests each module, they don't depend on each others much
      - hence you could easily create unit tests, which are often simpler and easier to specify than integration tests
      - it's recommeneded unit tests should part of the build process
    - #todo example of how it's easier to tes
- Developers are familiar with the importance of orthogonal system, but they often use terms like "modular", "component-based" or "layered" systems.
- A Layerd appraoch is nice because each later only relies the abstractions (API) provided by the layers below it. So there is a reduced risk of runaway dependencies.
- "dependencies" here basically means importing something from another module or some shared state, etc.
- 🗨 e.g. the the routes in your backend would depend on a "controller" layer where you implement the logic, and the controller would depend on the database layer (repositories). But the backend routes would not use call the database directly! It must go through the controller.
- 🗨 There is a nice package that let's you define the valid dependencies in your project called `dependency-cruiser`. You can use a `pre-commit` hook (basically a bash script) and whenever you commit it will verify all your imports and check if they don't violoate the architecture you created. e.g. if the route `/api/products` imports `ProductsRpository` and calls `productsRpository.getAll()` that would error out. You can only call `productsController.listProducts()`
- How to test if your design is orthogonal: ask yourself "If I drastically change the requirements for some functionality, how many modules will be affected"? The answer should _one_ (of course you realistically more than one module will be affected, but in you look carefully you should find that the changes truly related to the functionality happened in one module)

- avoid global data as much as you can.
  - 🗨 putting global variables in a JS module might create un ncesariy linkage.
- e.g. in Java people might use singletons to create global patterns, it might create unncesariy linkage

sections to re-read:

- orthogonality

- writing unit tests is a good test for orthogonality, if when you're writing a unit test for a module you find yourself importing so many other things, it means the module you're testing isn't well decoupled.
- fixing bugs too are a good way to assess it. you can see how localized the bugfix is, that is, if fixing an issue causes you to modify so many files, that's a bad sign.
  - tag bug fixes in git 🗨 i.e. the commit message e.g. use convention like `fix: some problem`
  - you can later create monthly reports analyzing the number of affected files in the bugfixes. you could get some good insights.
  - #todo
- DRY focuses on the duplication of knowledge, while orthogonality is about interdependency between modules. They are closely related. Because at the end of the day, it's all about ETC, we just want to reduce the pain of change.

🗨 **Assignment**:

- command line tools vs GUI[^gui] tools as software:
  - which are more orthogonal?: in terms of software design, command line tools win. we can combine them easily (e.g. using pipes) because they are completely independent and a proof of this is how some command line tools can be used in ways the author had never even imagiend. each process just outputs some string and it doesn't care what you do with it. Each command often focuses on completing one single task (e.g. grep for searching in files)
  - GUI tools, as software, aren't very orthogonal, often they do so many things and have a UI, so updating a feature might introduce changes in UI or other places. And from the user persepective they are harder to combine with other tools.
  - It's also much easier to build your own custom command line tools and combine them with the rest of the commands, unlike GUI tools.
    this is actually really interesting, because this is really what orthogonality is about. reducing dependencies as much as possible.
    This is an example from the book: for instance let's say want to go over a file line by line and split it into fields.
    you could write

```ts
class Split {
  constructor(filename: File) {...}   // open the fle
  readNextLine() {...}          // move to the next file
  getField(n) {...}             // get nth field in current line
}
```

🗨that isn't very orthogonal because you are assuming the input will always will come from a file, now imagine this class grows and becomes quite complicated, having tens of functionalties, then suddenly you realize you don't want to read the lines from a file. all the code that was using this class was using `readNextLine` and expecting a behavior, but it's like a "leaky abstraction", now you're stuck with it. like a GUI.
a better approach would be like this:

```ts
class Split {
  constructor(line: string) {}   // takes a string
  getField(n) {...}             // get nth field in the string
}
```

now if you can use this anywhere, you for instance read a file, go line by line and call this class, but now there ist's not coupled. you can use this the way you want. like a command line.

🗨 **Assignment**:

- todo: multiple inheritance vs multiple interfaces vs mixins
- thoughts: delegartion "has a" seems more orthogonal than "is a", something beings something else sounds complicated :D

data and transformation

a class couples code to data, often a code thing (cohesive)
but if you're not careful it can lead to ugly interfaces.

in FP languages it is encouraged to create small decoupled functions that take some data and output some data, and you can combine those functions. It's often good. But that can introduce some coupling so if you change data shape of some function you have to make sure it doesn't break other things
hmm... I need to think about this

### 11. Reversibility

- 🗨 Remember, good software is pretty much all about ETC, easier to change. the world is always changing.
- You won't always the best decisions, you might pick a database from some vendor[^vendor] (let's say MySQL or Postgres) then at some point you realize it's too slow for your use case, so want to switch to a document database (let's say Mongo). But you're mid project now, if you haven't been writing code that is reversable, you're out of luck.
- 🗨 You know, I feel is is a humbling idea, that you don't trust your capacity, you're a human being, you won't always know the right thing to do, hence the best you can do in such a world is to write code that is easy to change.

The way it's implemented is using the _Repository_ pattern (sometimes called DAO in the Java world) the idea is so simple, you'd make an interface `ClientRepository` containing all the mothods you need,e.g. `save`, `update`, `getAllByName` or whatever you need. Then you'd implement it. You'd create a class `PostgresClientRepository` and implement it. You can instead use an ORM like Drizzle which abstracts many SQL details so that it's so easy to switch between realtional databases. so you'd have `DrizzleClientRepository`. Now if you want to switch to Mongo, you'd just create `MongoClientRepository`. But how is that helpful?
Main idea: the application code should not know how it gets the data, use the interface to abstract it away.

```
functoin getClientRepository() {
  return new PostgresRepository()
}
...
GET("/api/client", (request, response) => {
  ...
  let service = new GetClientService(getClientRepository())
  return service.execute()
})
```

we created the `getClientRepository` so we have a single point from which we can change all repositories, we can simply return `MongoClientRepository` if we want.

- [ ] todo: create a very simple app using postgres then change it to use mongo

This approach is also nice for testing! You can easily create `InMemoryClientRepository` that implements ClientRepository, and test the use cases using it. So you'd create unit test for `GetClientService`, but instead of passing a postgres client repository, you pass the inMemory one.

BUT, I find it annoying because now whenever you update the PostgresRepository, you also need to remember to update the inMemory one. an integration test using the real database seems to make more sense to me. But unit tests using InMemoryClientRepository are honestly so dang fast and they do catch problems.

> Tip 18: There are no final decisions

- Don't assume things will stay the same, one day the client wants a web app, tomorrow he might want a mobile app. databases change, libraries changes. Your code must be able to adapt.
  - 🗨 [Interview with Senior JS Developer 2024](https://youtu.be/aWfYxg-Ypm4?si=8mJxm35_zv58stuT)
  - "Don't write this down, next week all of this is gonna change" :D
- Software architecture is constantly changing, trends change so fast. The best you can do is making sure your software is adaptable, that it's easy to change and reversible.
- Always wrap third-part APIs behind your own abstraction layers.

> Tip 19: Forgo Following Fads

### 12. Tracer Bullets

- soldiers use tracer bullets to help us hit targets because they offer immediate feedback, it makes it easier to see if you hit the target or not.
- we also needs such tracers in software development; basically we want to see if we're hitting or not, are we going in right direction?
- You would do this by choosing some important feature
- Since configuration and project setup is complicated these days, especially with the number of dependencies, The first useful tracer is usually just getting the project to work, end to end, all the layers are working fine and integrated.
  - That's very helpful for the team too, having a structure to work with it much batter than staring at an empty code base. It improves everyone's productivity.
- 🗨 Is the gun even firing, it doesn't matter if we hit the target or not, I just want to see it firing. I want to see the first tracer!
- 🗨 I love doing this too, though usually at a small scale, for instance if I need to implement a new feature I'd start with defining the API route, then creating stubs for the service or buisiness logic, and connect it to the data layer, and also create a stub for the its functions (e.g. simply returning an harcoded object instead of fetching something from DB). I find doing so reduces the cognitive charge and help me start to understand the new code base I'm working on. And It's much easier to sport mistakes at that time because the code is usually simple and small.
- Pragmatic Programmers take it to the next lever and turn it into a development style, you are activly shooting the tracer bullets and adapting. Basically whenever you feel you don't know what to do, pick some important feature and code it up, end to end, it doesn't have to work correctly but it should just work end to end, somethign you can show to users and your team and get feedback.
- Instead of solving the problem of not knowing where to look at in a dark by specifying the system to death, just use tracer bullets, shoot some shots, they won't always hit the target at first, but at least you're seeing something: it's always good to see something running end-to-end early.

> Tip 20: Use Tracer Bullets to Find the Targets

### 13. Prototypes and Post-it Notes

- prototypes can target specific aspects of a project
- in all fields, prototypes are great because they expose risk early at a reduced cost. After that, _you throw the prototype away_.
- not all prototypes are code based, you have a lot of options, you could draw a UI on a whiteboard, on some painting program, or some tool (🗨 e.g. Figma), etc.
- post it notes are good for prototyping dynamic things like application logic
- 🗨❓ not sure why post-it notes exactly, and no idea how they can be use it in this context, why not just a pen and paper?
- prototypes are great for things you aren't sure about and that carry risk.
- you can prototype a new functionality in your system, architecture, UI, performance issues...

> Prototype to learn

- it's not about the code you wrote, it's about what you learned while prototyping.
- you might want to use a high level scripting language like Ruby or Python (or JavaScript) for prototypes
- 🗨 This has something to do with _dynamic typing_, they won't get into your while prototyping, as there is no type checker to complain!
- 🗨 FYI there is no defintion for what constitute _scripting language_, but among friends it's basically a dynamic lanaguge that usually has tons of util functions, where it's easy to create short scripts that deal with files, etc. Python is known for this. It's _not_ about being interpereted or not, that's a very confusing and misleading idea.
- 🗨 Some consider scripting language to equal "interpreted", as opposed to "compiled" languages like C# and Java. And while that's fine, you can define terms as you wish but it can be misleading.
- Remember, prototypes will be thrown away later, it doesn't matter which language you use to create them.
- To prototype architecture you write code, but you can also can simply use a whiteboard with some post-it notes or index cards
- When you are building a prototype _make sure_ to make it so clear that the code is disposable and will not be used for further development. It's easy to get mislead by the apparent completeness of a prototype.
- If there is a risk people will still misunderstand the purpous of the prototype, well you may be better off without it and use an approach like Tracer Bullets.

### 14. Domain Languages

> The limits of language are the limits of one's world - Ludwig Wittgenstein

- 🗨 This fun topic to think about: how language can affect how understanding... remember 1984's Newspeak language which had deliberately a limited vocabulary to limit the citizen's thoughts? well that's an extreme version that linguists wouldn't probably agree with today, but I believe the idea that language can influence how we think does make sense.

- Computer Languages influence how you think about a problem. Solving a problem with C++ will have different result than approaching it with Haskall.
- The language of the problem domain can also be used!

> Tip 22: Program Close to the Problem Domain

- 🗨 Domain Specific Languages (DSL) are everywhere! I bet you already know many! Open any modern web development project and you'll see it full of such small languages.
- 🗨 CSS is not a programming language, it's a language made for a specific task, styling a web page. That's why we can call it a domain-specific language.
- 🗨 _domain-specific language_ (DSL) isn't a great term. I read in Crafting Interpreters that they used to call them little languages. I think _domain Languages_ is fine though.
- 🗨 RegEx is a domain language too, it has a specific use: matching strings with patterns.
- 🗨 A Dockerfile is a DSL.
  #todo add example here
- 🗨 Same for docker compose

- 🗨 You just describe the steps, and it works
- 🗨 Same for makefiles
- 🗨 SVG is a DSL for drawing images

```xml
<svg width="100" height="100" xmlns="http://www.w3.org/2000/svg">
  <circle cx="50" cy="50" r="40" fill="red" />
</svg>
```

- 🗨 This is a language for linear programming called OPL:

```
maximize 50 * x + 30 * y;

subject to {
    2 * x + 1 * y <= 40;   // labor constraint
    4 * x + 6 * y <= 120;  // material constraint
}
```

- 🗨 Another neat example I saw was a [domain language for editing videos](https://github.com/missing-semester/videos/blob/master/src/msv/lectures/iap2026/lec1.py) that was used to create MIT's The Missing Semster course.
- Ngnix (a web server) has a DSL for server configuration.

```
http {
    server {
        listen 8080;
        root /var/www/html;
    }
}
```

- 🗨 Testing libraries like Jest and Vitest often come with pretty nice syntax that lets you focus on tests. It's a beautiful abstration. And I think it can be considered a DSL.

```ts
describe("sum function", () => {
  it("should add two numbers correctly", () => {
    expect(sum(2, 3)).toBe(5);
  });

  it("should handle negative numbers", () => {
    expect(sum(-1, -1)).toBe(-2);
  });
});
```

Some languages take it to the next level, cucumber is testing library that lets you write tests in an even more readable format.

```
Feature: Sum function
  As a user
  I want to add two numbers
  So that I get the correct result

  Scenario: Add two positive numbers
    Given I have numbers 2 and 3
    When I add them together
    Then the result should be 5

  Scenario: Add two negative numbers
    Given I have numbers -1 and -1
    When I add them together
    Then the result should be -2
```

- Yup, you can actually execute that test! (you add more config files of course)
- Cucumber was initially made so that business users can read the tests, but that rarely happens.
- one reason "gather requirements, design, code, ship" approach doesn't work because we rarely know what the requirements are! the business users will have a vague idea of what they want, they don't know nor care about the details.

> That's our value: we intuit intent and convert it into code

- That's why it's not a good idea to have them read such tests, give them some prototype or some running code and you'll get much better feedback.

- There are two kinds of domain languages: Internal and External
- Internal are language written in the host language, e.g. Jest tests, they extend the host language.
- Ruby is known for being one of the best languages for internal DSL, look at how pretty and elegant this code is:

```ruby
describe "Calculator" do
  it "adds two numbers" do
    expect(2 + 3).to eq(5)
  end
  it "subtracts numbers" do
    expect(5 - 3).to eq(2)
  end
end
```

- External DSLs are have their own language, their own synax, which gives them more freedom to create any fancy syntax. Hence they usually have their own _parser_ that turns that code into some data structure and then execute some functionality.
- _parsing_ is a very useful term to know: the parser receives some string, it turns it into a data structure. that's it. that's a parser. it knows the syntax rules, and based on them it will parse the srting. The same way HTML file (a bunch of text on the disk) is turned into a DOM tree in memory that you can manipulate (and the browser would display).
- This is true for external domain languages too, they are parsed by a program and that program does the magic, it abstracts all the details from you and lets you use the language of the problem. The nice thing about external language is that you can come up with any syntax you want, there is a lot of freedom.
- You can write your own parser for a DSL, e.g. let's say you want to have a language for HTTP configurations, let's say you come up with this syntax, and let's call this language YACL (yet another config language!)

```
listen on port: 8080+ // if 8080 is taken try 8081, etc.
dir: /html/project
logging: off
```

- But good luck writing a parser, though there are many great tools that can help you (there are parser gernerators, in fact some let you define the syntax rules for your parser using a domain langauge, now isn't that cool!), but it's still not really that easy, and it could be time consuming.
- The parser would _open_ that file we wrote, then with some magic (take a compilers class or read Crafting Interpreters if you want to know how) it outputs a data structure, e.g. a Javascript object:

```js
{
  port: 8080,
  incrementPortIfTaken: true,
  dir: "/html/project",
  logging: false
}
```

Instead of writing your own praser you could instead use external languages like XML, JSON, or YML to create your own domain languages. It's not as pretty and expressive but it's good enough. well in our case, you can simply put the exact same object in a JSON file, or even keep it as JavaScript, that's how so many JS libraries handle configurations!

```json
{
  "port": 8080,
  "incrementPortIfTaken": true,
  "dir": "/html/project",
  "logging": false
}
```

- You could also use XML thought it's often not recommended for configuration, because it's so ugly. Though it's pretty good as a markup language.

- Again, you don't have to write your own parser! you can also use languages like XML and YML, which already have battle-tested parsers ready to use. The parser would parse the file and give you a data structure then you can do whatever you want with it!
- Let's say you want a DSL to run a small robot you have, you can define a language for it in XML:

```xml
<steps unit="cm">
  <moveUp dist="20">
  <moveLeft dist="50">
  <turnOff/>
</steps>
```

- You can then write code to parse this file and you write code to move the robot based on the tags.

- All of this helped me internalize the idea that everything is pretty much a bunch of files, software is just a bunch files!

#TODO: do the problem set in this section

### 15. Estimating

- 75TB of data, over 1Gbps network?
  - 75\*2^40\*8 / 2^30
  - 🗨 btw I found these numbers useful to remember:
    - 10^3 (thousand - kilo) is approximately 2^10
    - 10^6 (million - mega) is approximately 2^20
    - 10^9 (billion - giga) is approximately 2^30
    - 2^10 bit = 1Kb (1024 bit) [Kb isn't same as KB]
    - 2^20 bit = 1Mb
    - 2^30 bit = 1Gb
    - it's often recommended to memorize the powers of 2 (up to 2^15)
    - How much is 2^25 bits? well around 32Mb

- how much storage you need for a million names and addresses
- how long does it take to compress 100MB of text?
- You should learn how to estimate to have a sense of the magnitude of things

- at one level the answers here don't really matter.
- but learning how to estimate as developer, to the point where you have intuitive feeling for the magnitude of things, can you have deeper understanding and the feasability of options.

> Tip 23: Estimate to Avoid Surprises

- Context matters, the accurace of estimates differs based on the situation.
- People will understand your estimation differently based on the terms you use, if you say the project will take 130 working days people will expect something close to that. And if you say it would take 6 months --even though it's the same period -- people will have different expectations.

- Estimations are based on the models we have for problems. You don't have to immediately start buildinga model; The best first step for good estimates is simply to ask others who have been in a similar sitation or solved a similar problem.

#TODO: re-read this section - still didn't fully get it.

## Chapter 3: The Basic Tools

### 16. The Power of Plain Text

> As programmers our base material isn't wood or iron, it's knowledge

- plain text is the best way to store knowledge persistently
- In binary formats (as opposed to human-readable formats) the context is separate from the data, you can't understand the data without the program or software that opens the file and parses it.
- plain text is simply any file containing text; ASCII/UTF-8 characters, etc.
  - basically any file you can open it with notepad and understand its content.

> Tip 25: Keep Knowledge in Plain Text

- For instance, writing documents in MD files is much better than writing in some word precessor like microsoft Word[^word]
- plain text doesn't mean it's unstructured: HTML, XML, Markrdown and JSON are all plain text
  - 🗨 sometimes called "semi-structured" files
- There are three reasons why plain text is awesome
  - 1. Insurance against obsolescence: plain text survives. For binary files you would need to know everything about the file to parse it.
  - 2. Leverage existing tools: you can do anything with plain text
    - you can `grep` a text file
    - you can version control it easily
    - you can `diff` it

- plain text is really awesome because once parsed, you can do whatever you want with it, that's why static site generators do for instance, they allow you to write MD files then they get converted to HTML.
- and the nice thing about it is that you can customize how to display it, for instance if you write a document using MD you can display it differently (e.g. I use Obsidian to write MD files and I can easily change the theme and install new ones)
- 🗨 It's worth understanding what is plain text, I've noticed some people don't quite understand how text is represented
  - I recommend this article #todo: add it here later
- Binary files have their advantages too, they are often more efficient
  - if you write "27500000" in JSON, that's 8 bytes of data, you can store the same number (and larger numbers) in a binary foramt usnig 4 bytes. That's why in databases they don't store information as plain text (e.g. Mongo uses BSON format) and binary formats are efficient for other reasons.
- 3. It's easier to test

> If you use plain text to create synthetic data to drive system tests, then it is a simple matter to add, update, or modify the test data _without having to create any special tools to do so_.
> ❓ I don't quite understand what this means.
> in integration tests I often find myself needing to re-set the database state to a specific state, maybe I can create multiple JSON files representing different states of the DB and maybe create some abstraction that would take a file and set the DB to it.
> I once did a similar thing but it was for an XML database called XState... But I'm not sure this is what the book is talking about.

> Even in the future of blockchain-based intelligent agents that travel the wild and dangerous internet autonomously, negotiating data interchange among themselves, the ubiquitous text file will still be there.

### 17. Shell Games

- 🗨 I was raised on GUI so personally it took me a while to understand how powerful the shell is.
  > A benefit of GUIs is WYSIWYG—what you see is what you get. The disadvantage is WYSIAYG— what you see is all you get

> Tip 26: Use the Power of Command Shell

- 🗨 MIT's The Missing Semester is a great course to get into the shell. I learned so many useful commands from it.

- 🗨 if you feel you don't like the shell, I higly recommand that you try the `zoxide` command and `tmux`, these two made me fall in love with the shell.

### 18. Power Editing

> Tip: Achieve Editor Fluency

- You need to reach the point where you edit the files effortlessly, you don't even need to think about it.
- 🗨 I think you should simply put some time to learn your editor well; I once heard Lex Fridman explaining how editors like VS code don't are so easy to start with that you don't have to learn them. You can spend years using VS Code without learning how to use it effectively. while if you can't even use Vim without learning it well. So we should learn our editors.
- Here is a nice video from Syntax about nice [vscode tips](https://youtu.be/c0HO_-NDJCk)
- One ther thing I frequently use when editing.
  - grow/shrink selection `Alt + Shift + RightArrow/LeftArrow`: This one is great, in JS you often want to select all lines between two parenthses or brackets, this command allows you to do that easily.

- You don't need to know all the features and deatils. The recipe for becoming better at editing is fairly simple: just look at yourself while editing, if you notice you're repeating something over and over then you need to think "there must be a better way".
- exetend the abilities of your editor. There are many good extentions for ecosystem you're working on.
- learn how to use your editor's extension language to automate reptitive things
  - 🗨 learn how to create snippets in VS Code
  - if needed you could even build full extensions and share them with others.

### 19. Version Control

> 28: Always Use Version Control

- use version control for _everything_, it doesn't have to be code.
- learn how to recover from disasters, how to fix mistakes. Many people use git and know that git can help them in disasters but actually never found the time to learn it well. You should learn it.
  - 🗨 I really love the Head First Git book, it teaches well how to fix mistakes with git.

- imagine you lost your computer, how fast would it take you to set up a new computer - with all your aliases, settings, apps? most configs are stored as plain text, so you can use git to manage this.
  - 🗨 many people use symbolic links and create a dotfile repository which contains all their configurations like `bashrc`, `.tmux.conf` and so on. you can also create scripts that would copy configuration files to their correct place, and much more.
- find another computer you no longer use and test how fast can set it up to see if your recovery system works.

> Version control branches and test organization have something in common: they both have thousands of people out there telling how you should do it. And this advice is largely meaningless.

- 🗨 one of the things that often surprised me when I started out in web development. There are so many approaches for problems and in many cases there is no consensus.

> IF 1000 SOLUTIONS EXIST, NO GREAT ONE DOES - Operating Systems: Three Easy Pieces

### 20. Debugging

> Tip 29: Fix the Problem, Not the Blame

> It doesn't matter if it's your fault or someone else's. it's still your problem.

- You might feel stressed, having a deadlines and preassures. You should relax, and focus on solving the problem.

> Tip 30: Don't Panic

- Don't waste time thinking that "it's impossible" for this error to happen. because it can.
- Don't just fix what appears to be the issue, you just modify the code, run it, get some other errors, fix them, run it, the code works and the test pass. That's it. You should try to find the root of the problem, not just one appearance of it.
- after understanding the bug, start by re-producing it. We want a bug that can be reproduced with a single command. So write some test that would reproduce the bug.

> Tip 31: Failing Test Before Fixing Code

- Just the act of writing the test itself might help you think more deeply about the problem.
- If it's a crash, just...

> Tip 32: Read the Damn Error Message

- if it's not a crash, if it's wrong output, use a debugger and trigger the error with your failing test.
  - 🗨 simply put a 🔴 breakpoint on the failing test and run it in debug mode.
  - learn how to use an interactive debugger if you never used it.
    - learn how to debug react code
    - learn how to debug node apps
- Make sure you know how to move up and down the call stack
- Keep a pen and paper and take notes, for example sometimes you might find a clue and chase it down but it turns out not the issue, if you didn't take some notes where you were before it takes more time to get back where you were before.
- Use the _binary search_ technique (aka binary chop) technique while when faced with a huge stacktrace and you want to know which function cause the error.
  - #todo: example
- same goes with datasets, if you have a test dataset that made your test fail, divide the data see which part made it fail. and so on.
- If you your team created a bug at some point but you aren't sure when. you can create a quick test that triggers the bug then choose a release in the middle between the oldest known working version and the neweset release.
  - 🗨 basically, learn how to use `git bisect`
  - you have a project that has these commits: `... - (✓) - (?) - (?) - (?) - (x)`
  - suddenly you realize there is a bug in the latest commit... but you don't know when the bug was introduced, it was added by someone at some point and we didn't realize it...
  - but you know for sure that some release had no such bug, let's say in the first commit
  - no imagine there are hundreds of commits between them! you can't just keep checking them one by one! and so we use the binary search technique (git automates it using `git bisect`)
  - 🗨 don't commit the test you just created, so that you can run the test each time. remember, git will keep untracked files when you switch HEAD to point to a different commit.
  - 🗨 git takes it to another level by letting you running the test automatically and deciding based on the test result. while you drink your cup of tea or coffee.
  - 🗨 this also work for UI bugs, at each time you switch release, you can run the project again and manually test with the browser if it works as expected.
- tracing statements (🗨 i.e. printf debugging) is very useful sometimes, especially when time itself is a factor that can help you understand the problem. that is, when you need to watch the state of the application change over time. This is especially true in event-based systems, concurrent processes and real-time systems.
  - ❓ "event-based systems": I got to learn something about event-driven architectures, I know the idea of events (often used in game development) and the idea of events and callbacks in web development which is similar. And I once learn a bit about IoT and how sensors register events in a broker. But I never implemented such architecture myself. Seems like an cool topic.
- Rubber ducking (aka Rubber Duck Debugging)
  - 🗨 talk about a grudge against the language
  - explain the problem to another person, you'll be surprised how helpful it is to put your understanding into words. if you don't find a problem you explain it to a rubber duck, or a teddy bear, or whatever you find in front of you!
  - 🗨 I got to say, moments like this make me feel glad I got myself into this weird profession of programming.

- When something goes wrong, first always assume the problem is in your code, and most likely it is. even though there is a small chance it's due to the OS update, or the DB is broken, or mabye the JS package got it wrong. but that's often not the case. So always start by doubting you code. The OS probably is not broken. you code is probably is.

> Tip 33: "select" Isn't Broken[^broken-select]

- Some bugs will surprise you, "it's impossible" you'd think. but alas, it happened.
- Don't assume a piece of code will NEVER be a source of bugs, of course it can.

> Don't Assume It - Prove It

- when you find a bug don't just fix it:
  - ask yourself why didn't you catch it earlier? maybe you need to improve the tests? so that they can catch such bugs earlier.
  - see if any other places in code are susceptible to similar issues

### 21. Text Manipulation

- This is serious: programmers manipulate text the same way wood workers manipulate wood.
- You go to learn some text manipuation languages, they are extremely useful. But like any great tools they take time to master.
- you can use built-in shell tools like `sed` and `awk`. you can also use Python or Ruby if you prefer a more structured language.

> Tip 35: Learn a Text Manipulation Language

- 🗨 The `awk` is one of my favorite commands, it's super useful in so many different ways.
  Let's say I have this folder structure

```
- Country 01
  - Bank 01
    - 2010.pdf
    - 2011.pdf
    ..
  - Bank 02
    ...
- Country 02
  ...
```

I wanted to check if all files are named correctly, I wanted to see if there are files names that aren't `[year].pdf`
Pseudocode:

```shell
find . -type f -name "*txt"
| awk -F '/' '$NF !~ /[0-9]{4}\.txt/ {print}'
```

you feel you can do whatever you want with the text, as long as the text has some structure, you can mold it the way you want. The feeling it gives you is really hard to describe.

challenge #todo: write a script to turn a directory of YML files to JSON files.
challenge: you decided to move from camelCase convention to snake_case for variables, write a script that goes over that scans your codebase for any camelCase variables and report them to you.
challenge: add the ability to change those variable names in one or more pages. (make a backup of your files, something might go wrong!)

### 22. Engineering Daybooks

- A journal where you record what you did and learned. where you sketch ideas, plans, etc.
- you can use it to take notes in meetings, to note down variable data when debugging, doodling.
- it has many benefits; at some point you'll have a bunch of daybooks and you could go over them and see the projects you were working on them and the problems you faced.
- 🗨 I had a daybook for around a year now, I have been using it for some stuff, mostly for insights I learned from courses. Database tricks I learned, shell commands. DNS records, quotes I like... It's really fun and I like doodling on it.

## Chapter 4: Pragmatic Paranoia

> Tip 36: You Can't Write Perfect Software

- we deal with others; We deal with a lot code that might not live up to our standards; so learn that it's important to program defensively, we validate everything, we never trust the data we get, we use assertions to detect bad data, we doubt and check
- pragmatic programmers take it to the next level: _they don't trust themselves, either_ because the know no one writes perfect software.
- 🗨 reminds me of Dijstra's wise words:

> We shall do a much better programming job, provided we approach the task with a full appreciation of its tremendous difficulty, provided that we respect the intrinsic limitations of the human mind and approach the task as very humble programmers

- 🗨 I think being honest about our human limitations and accept our own weaknesses is a virtue and it matters, I really like thinking. But what matters more is what you do with it. How you deal with those limitation and trying to do the right thing is the goal.

### 23. Design by Contract

> Dealing with computers is hard, dealing with people is even harder.

- Human beings figured that contracts can be a useful thing when dealing with others in some circumstances. you define the rights and responsibilities of each part, etc.
- We can apply this to software development (how modules interact). It is called **Design By Contract** (DBC).

focus on the rights and responsibilities of modules to ensure _correctness_
correctness = doing no more or less than what you claim to do
the heart of DBC: verifying and documenting that claim.

every function does something. and it expects some state of the world.

- preconditions: what must be true for the function to be called.
  it's the caller's responsibility to pass good data

- postconditions: what the function is guaranteed to do.
- class invariants: from the persepective of the caller, what will always remain true.

The contract:

> If all the routine's preconditions are met by the caller, the routine shall guarantee that all postconditions and invariants will be true when it completes.

- if either the caller or the function fail to meet this contract, something that you agreed to should happen, e.g. an exception is raised or the program terminates.
- failure to meet the agreement IS A BUG. it's something that should never happen!
  - that's why pre-conditions must never be used for something like input validation

> Tip 37: Design with contract

- You should be lazy: be strict in what you'll accept from the start and promise very little.
  - 🗨 "if you don't meet the terms of the agreement, well, I won't do anything, why do you expect me to bend myself forward and understand the heck you want"
  - this helps catching bugs early and write better software. You avoid _programming by coincidence_.
    > _DBC forces you to think_.

- It works in any programming language
  ❓ But wait... postconditions don't make sense in some cases, e.g. if you update the database, you need to rollback. well if you the function throws an error it should rollback.
- Class invariants is not just about OOP, it's just a term. The idea is about state and how you should never be in an invalid state after an operation. Other languages have state too, e.g. in FP you would pass the state to functions.
- it's actually ok to be in an invalid state while the function code is running, but at the end the invariat must hold true.

- But don't we write tests anyway?
  - DBC and testing are both useful, but DBC has its own unique strengths
  - DBC doesn't require any setup or mocking, testing might miss cases while DBC claims are always there, at runtime, even in production and maintenance phases.
  - Testing is good of course, and approaches like Test Driven Development is a great technique but it might make you focus too much on the "happy path" and miss some cases.

- Some languages would help you automatically check your contract (e.g. Eiffel, Clojure);
- But just thinking about the input and what the function promises to do, and more importantly, what it doesn't promise to do, _before_ writing a single line of the function: that alone is a huge step towards better software.
- Even without automatic checking if you just _think_ you did well. You can put those contracts in comments or in a unit test.
- It would also be great if you can statically check those contracts, but you can emulate this partially by runtime checks: assertions.
  - DBC style checks run even even before the function body is executed. assertions are in the function body.
  - Assertions sometimes can be turned off, which is a problem.
- It's not as powerful as languages that fully support DBC, but it's better than nothing.
- ❓🗨 Why don't we just throw an exception? assertions themselves throw an exception...

```ts
const sqrt = (x: number) => {
  if (x < 0) {
    throw new InvalidInput('sqrt expects a nonnegative number')
  }
  ...
}
```

But using asserts seems like a better idea.

```typescript
const sqrt = (x: number) => {
  assert(x >= 0)
  ...
}
```

- Both will throw an exception, but it seems asserts communicate the contract, it has a more semantic meaning than simple error throwing, it also looks like DBC clauses in Eiffel and Clojure. So it seems like the better way to emulate DBC.
- Again, if the pre-conditions fails IT IS A BUG. It's something that should never have happened. It's the calling side's problem for not meeting the agreement's terms. The function is not responsible for the failure.

- Semantic Invariants: kind of "philosophical contract"
- Use it for requirements that are essential to the very meaning of something, not "fixed" requirements, even those might change. But some requirements might qualify to be "semantic requirements".
  - When you find such invariants make sure to document it well and maybe even write it on a whiteboard so everyone sees it.

- ❓ The book has a short section about autonomous agents and dynamic contracts... it didn't fully understand it.

- Why isn't DBC more common? Because it forces us to think about problems we'd rather ignore for now. Because it forces us to _think_.

> Clearly, this is a dangerous tool

### 24. Dead Programs Tell No Lies

all switch cases should have a default case / let us know when the impossible happens
falling into "it can't happen" mentality

> Tip 38: Crash Early

> Defensive Programming is a waste of time, let it crash - Joe Armstrong, inventor of Earlang

- A Dead Progeam does much less damage. Continuing to run in an invalid state might create really big problems.
- Sometimes it might not be appropriate to terminate; e.g. in a web server; you might need to add some logging and clear up the used resources, etc. what matters is that you don't continue to run in a bad state.

### 25. Assertive Programming

> Tip 39: Use Assertions to Prevent the Impossible

- whenever you feel "but this would never happen" add code to check it.
- you should add a custom message

```ts
const assert = require('node:assert');
...
assert(currentStatus === 'pending', 'The current appointment state is not pending');
```

- Do not use assertions in place of real error handling
- The following is a BAD IDEA:

```ts
const answer = readInput();
assert(answer === "Y" || answer === "N");
```

- Asserts are for the things that SHOULD NEVER HAPPEN.
- You can catch the assertion exception and clean up resources.
- _Leave asserts on in production._
- You can display a nice UI to the end user when an assert fail and report the data, this can help you build robust software and find the subtle bugs that are hard to find and reproduce.

### 26. How to Balance Resources

### 27. Don't Outrun Your Headlights

## Chapter 5: Bend, or Break

### 28. Decoupling

### 29. Juggling the Real World

### 30. Transforming Programming

### 31. Inheritance Tax

### 32. Configuration

## Chapter 6: Concurrency

### 33. Breaking Temporal Coupling

### 34. Shared State Is Incorrect State

### 35. Actors and Process

### 36. Blackboards

### Chapter 7. While You Are Coding

### 37. Listen to Your Lizard Brain

### 38. Programming by Coincidence

### 39. Algorithm Speed

### 40. Refactoring

### 41. Test to Code

### 42. Property-Based Testing

### 43. Stay Safe Out There

### 44. Naming Things

## Chapter 8. Before the Project

### 45. The Requirements Pit

### 46. Solving Impossible Puzzle

### 47. Working Together

### 48. The Essence of Agility

## Chapter 9: Pragmatic Projects

### 49. Pragmatic Teams

### 50. Coconuts Don't Cut It

### 51. Pragmatic Started Kit

### 52. Delight Your Users

### 53. Pride and Prejudice

## Footnotes

[^think]: It's worth noting that this is not at odds with trying things out when you're trying to understand the problem; sometimes it's a good idea to start getting your hands dirty and start with some code, or come up with examples when you're trying to solve a math problem. The problem is when you start to get into autopilot mode and enter what I like to call the WHEEL loop (write, hope, execute, errors, loop)

[^latex]: Pronounced as /latek/

[^api]: This term is used in many different contexts; it's not just about web APIs; it could mean a bunch of library functions that you can use without needing to think about how they work inside. You just need to understand the expected inputs and outputs. So when you hear the term think of a JS module exposing some functions, those functions are the API of that module.

[^exported]: i.e. library functions you can import from somewhere else, let's say I create a module in JS (i.e. a JS file) and created some logging or security functions, when I use the export statement people can import them from other places and use them.

[^cohesion]: "cohesion refers to the degree to which the elements inside a module belong together." - Wikipedia. The books says "when coupling is good, we call it cohesion"

[^component]: software components. it's basically like a module in JS, it's a very general term. anything with some implementation and an exposed API.

[^GUI]: many pronounce it as "gooey"

[^word]: btw Word now stores files as XML under the hood, but it's not a human readable format, its' just because Microsoft was required -legally- to allow interoperability with other word processing tools.

[^broken-select]: referring to a short story in the book when one programmer mistakenly believed that the `select` system is broken and refused any other explanation.

```

```
