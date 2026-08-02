# Pragmatic Programmer

Book by David Thomas and Andrew Hunt

## Table of Content

- [Introduction](#introduction)
- [Chapter 1: A Pragmatic Philosophy](#chapter-1-a-pragmatic-philosophy)
  - [It's Your Life](#its-your-life)
  - [The Cat Ate My Source Code](#2-the-cat-ate-my-source-code)
  - [Software Entropy](#3-software-entropy)
  - [Stone Soup and Boiled Frogs](#4-stone-soup-and-boiled-frogs)
  - [Good-Enough Software](#5-good-enough-software)
  - [Your Knowledge Portfolio](#6-your-knowledge-portfolio)
  - [Communicate](#7-communicate)
- [Chapter 2: A Pragmatic Approach](#chapter-2-a-pragmatic-approach)
  - [The Essence of Good Design](#the-essence-of-good-design)
  - [DRY - The Evils of Duplication](#dry---the-evils-of-duplication)
- [Footnotes](#footnotes)

## Introduction

> Programming is about making the future less painful – Saron Yitbarek

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

### It's Your Life

> Tip 3: You Have Agency

🗨 The book starts with some motivational speech - but it's not that annoying; it seems just some useful and pragmatic (= practical) tips the authors have learned over the years.

The authors have noticed that many programmers are very concerned and maybe feeling uncomfortable at their jobs or life, but they are doing nothing, even though this field is one of the best fields when it comes to agency; there are a million things you can do!

### 2. The Cat Ate My Source Code

Take responsibility for your mistakes and shortcomings.
It's not a fun thing to happen; it's not easy to admit mistakes, but in my opinion, I think it's honorable.
The book also explains that the team should be able to rely on and trust you. And that trust is built through action; a good team is a team built on trust and interdependence.

🗨 This, for some reason remind of the famous scene you see in too many films, 'It's not your fault'. As if being mistaken is something to be ashamed of. To me, a good friend or teammate is someone who'd tell you, 'Dude, you messed up, but it's okay; let's find a solution'.
🗨 I understand the culture we're starting to have, the culture of not naming things what they are. It's comforting, and there is nothing wrong with seeking comfort; we all do want that. But I think it's leading us to even worse environments.

Tip 4: Provide Options, Don't Make Lame Excuses

The section ends with a very practical tip: instead of offering lame excuses when something goes wrong, explain what can be done and offer different options.
Another pro tip: don't just say 'I don't know'; follow it up with 'I'll figure it out'

### 3. Software Entropy

- 🗨 Entropy here is the thermodynamic entropy and not Shannon's Entropy (Information Theory)
- Entropy in thermodynamics is a 'measure of disorder'. And by the laws of physics, any system tends toward the maximum entropy, that is, it tends towards disorder.
- When the software is chaos The author calls it a 'software rot'; they don't seem to be fond of the more optimistic term 'technical debt', because it implies the 'debt' will be paid back, but it often isn't the case.

> Tip 5. Don't Live with Broken Windows

- A broken window in a building is all it takes to instill a feeling that the building is neglected and slowly drives a feeling of hopelessness, and slowly the building will get worse and worse.
- Same goes for software (and many things in life): you should fix problems as soon as you find them, don't let them rot, at the very least show some effort, show that you care. Open an issue for the problem, add some stub 'not implemented yet' message, have a plan to refactor bad code, etc.
- The book claims that such small things, with enough time, are one of the reasons that could ruin even the biggest of projects. The effect of neglect compounds and changes how everyone feels about the project.
- 🗨 I've read that 'Broken Windows Theory' has not been proved yet and there are some discussions about it. But I like the advice, and I think it's valid. It's never a good idea to leave many 'open files' in the background. It's like having monsters lurking in the back of your mind!

### 4. Stone Soup and Boiled Frogs

Sometimes you know what the right thing to do is, something that will certainly benefit the project, but you'll have to ask for permissions, and it's not easy to convince others, or it takes too much time. The book recommends that in such case you should think of the simplest thing you can ask for and you won't get rejected, after that it's okay to try whetting others' appetite by showing them a 'glimpse of the future', basically saying 'Of course it would be nicer if we add add this or that feature', but pretend it's not that important and wait, there is a good change they would tell you to implement it.

🗨 This is a general social skill I someone taught me, that is, not trying too hard to offer what you have if the other part doesn't seem to care, like when you want to advise someone who doesn't seem to care, sometimes talking too much doesn't help and makes your words less meaningful, this is clearly true for school teachers for instance, the teacher's words might lose impact if they repeat it too many times. Sometimes silence could intrigue the student because it's different and makes them want to hear from you.

### Tip 6: Be a Catalyst for Change

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

### The Essence of Good Design

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

### DRY - The Evils of Duplication

- As programmers we care about _knowledge_, we document it in spec and implement it. Managing knowledge is part of our job.
- knowledge is constantly changing. you talk to the client or maybe some regulation changes, now suddenly the business logic is outdated.
- Maintenance doesn't start when the project is released, it's part of our daily work as programmers, we're constantly maintaining the code as knowledge and our understanding change day by day.
- It's easy to duplicate knowledge (in spec, code, etc), and it causes a maintenance hell.

> Tip 15. DRY - Don't Repeat Yourself

> Every piece of knowledge must have a single, unambiguous, authoritative representation within a system.

- what's the opposite of that? a single piece of knowledge having two representations. If you change one you need to change the other and that's not ETC.

> It's not a question of whether you'll remember: it's a question of when you'll forget.

- DRY is not just about code duplication (copy pasting code in many places)! it's part of it but DRY is much more than that. The real problem is expressing the same knowledge in many places.
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
- Sometimes youd find comments that are just re-stating the code logic and the steps done.
- 🗨 It occured to me that it's as if you're writing the program in two programming languages each time. It's as if you're writing the program in a DSL then writing it again in a programming language!
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

## Footnotes

[^think]: It's worth noting that this is not at odds with trying things out when you're trying to understand the problem; sometimes it's a good idea to start getting your hands dirty and start with some code, or come up with examples when you're trying to solve a math problem. The problem is when you start to get into autopilot mode and enter what I like to call the WHEEL loop (write, hope, execute, errors, loop)

[^latex]: Pronounced as /latek/

[^api]: This term is used in many different contexts; it's not just about web APIs; it could mean a bunch of library functions that you can use without needing to think about how they work inside. You just need to understand the expected inputs and outputs.

[^exported]: i.e. library functions you can import from somewhere else, let's say I create a module in JS (i.e. a JS file) and created some logging or security functions, when I use the export statement people can import them from other places and use them.
