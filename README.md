# Pragmatic Programmer

Book by David Thomas and Andrew Hunt

## Table of Content

## Introduction

> Programming is about making the future less painful – Saron Yitbarek

🗨 The book quickly mentions the issue of terminology, which I really enjoy

Either perfectly good English words that have been corrupted to mean something technical, or horrendous made-up words that have been assigned meanings by computer scientists with a grudge against the language

🗨 I'm not that attached to English as it's not my first language, but some terms really make you feel whoever came up with them really hated language. Memoization immediately comes to mind.

This book will help you become a better programmer.

🗨 The book is called Pragmatic Programmer, and the term pragmatism caught my eye because I know some philosophy. Pragmatism is a philosophy from the 19th century that had a great impact on the world; it has its unique epistemological basis (e.g., the nature of knowledge) and many concepts that all revolve around the idea of practicality; knowledge itself is judged by its practicality.

🗨 But when people say someone is pragmatic, they often don't mean the philosophy, but they simply mean the person is practical and gets the job done. So from what I understand, the book is not about philosophy; it's about the practical wisdom of two experienced programmers - though our philosophies and our values inevitably will affect our thoughts and our ink.

Tip 1: Care About Your Craft

🗨 The book's cover displays some carpenter's tools; this is related to the idea of craftsmanship and seeing your job as a craft you seek to master. Some people like this idea, and others would tell them to stop fantasizing! You're just a cog in the wheel. I think there is some middle ground. And I think it's also freeing to start treating it as a craft; it's not even about the joy you get, which is real, but realizing it's just a service sector; it's the same for doctors, carpenters, plumbers, etc. We're just offering a service that people need; it's not some heroic act to build software.

Tip 2: Think About Your Work

🗨 It's important to think about your work, and this reminds me of one quote by Dijkstra's that I heard in Remzi's operating systems online lectures. Dijkstra explains that experience is not the same as wisdom; to have wisdom, you need both experience and reflection. Constantly reflecting on your work, and more importantly, on yourself, your emotions, is a great path for growth. And it's not easy because most of us are very distant from ourselves and our thoughts.
🗨 When it comes to programming, I like to call it deliberate thinking; it's something I learned as a CS student by seeing it in different contexts and realizing its importance.
I've seen that even experienced developers do this. For example I've used to watch Ali Fadel, a software engineer who worked at Amazon, and made videos on competitive programming in Arabic.
One thing I kept noticing: he would explain a solution, and then pause and say 'now, why is that correct' or 'why is that not correct'. That made me reflect; I don't remember asking myself why a solution is not correct!

I have only one method that I recommend extensively—it's called think before you write. – Richard Hamming

'Think first, experiment later.'[^think] – CS2510

🗨 I remember now how in High School I used to find it odd that, unlike English essays, when writing French essays where we must start by explicitly writing the problématique, i.e., the problem we are discussing, I didn't realize then that it had some pedagogical reasons.

🗨The Book also points to an important thing, which is 'think about your work while you're doing it'. We often think we think 'We'll think about it later, I'll reflect later', but there are many things that could distract us, it's better to use every opportunity to reflect, and this a know fact in good learning which is to learn actively, instead of underlining or highlighting the book you're reading stop for a moment and try to recall the point the writer is making using your own words, try to think about it and critique it

## Chapter 1: A Pragmatic Philosophy

1. It's Your Life

Tip 3: You Have Agency

🗨 The book starts with some motivational speech - but it's not that annoying; it seems just some useful and pragmatic (= practical) tips the authors have learned over the years.

The authors have noticed that many programmers are very concerned and maybe feeling uncomfortable at their jobs or life, but they are doing nothing, even though this field is one of the best fields when it comes to agency; there are a million things you can do!

2. The Cat Ate My Source Code

Take responsibility for your mistakes and shortcomings.
It's not a fun thing to happen; it's not easy to admit mistakes, but in my opinion, I think it's honorable.
The book also explains that the team should be able to rely on and trust you. And that trust is built through action; a good team is a team built on trust and interdependence.

🗨 This, for some reason remind of the famous scene you see in too many films, 'It's not your fault'. As if being mistaken is something to be ashamed of. To me, a good friend or teammate is someone who'd tell you, 'Dude, you messed up, but it's okay; let's find a solution'.
🗨 I understand the culture we're starting to have, the culture of not naming things what they are. It's comforting, and there is nothing wrong with seeking comfort; we all do want that. But I think it's leading us to even worse environments.

Tip 4: Provide Options, Don't Make Lame Excuses

The section ends with a very practical tip: instead of offering lame excuses when something goes wrong, explain what can be done and offer different options.
Another pro tip: don't just say 'I don't know'; follow it up with 'I'll figure it out'

3. Software Entropy

- 🗨 Entropy here is the thermodynamic entropy and not Shannon's Entropy (Information Theory)
- Entropy in thermodynamics is a 'measure of disorder'. And by the laws of physics, any system tends toward the maximum entropy, that is, it tends towards disorder.
- When the software is chaos The author calls it a 'software rot'; they don't seem to be fond of the more optimistic term 'technical debt', because it implies the 'debt' will be paid back, but it often isn't the case.

Tip 5. Don't Live with Broken Windows

- A broken window in a building is all it takes to instill a feeling that the building is neglected and slowly drives a feeling of hopelessness, and slowly the building will get worse and worse.
- Same goes for software (and many things in life): you should fix problems as soon as you find them, don't let them rot, at the very least show some effort, show that you care. Open an issue for the problem, add some stub 'not implemented yet' message, have a plan to refactor bad code, etc.
- The book claims that such small things, with enough time, are one of the reasons that could ruin even the biggest of projects. The effect of neglect compounds and changes how everyone feels about the project.
- 🗨 I've read that 'Broken Windows Theory' has not been proved yet and there are some discussions about it. But I like the advice, and I think it's valid. It's never a good idea to leave many 'open files' in the background. It's like having monsters lurking in the back of your mind!

4. Stone Soup and Boiled Frogs

Sometimes you know what the right thing to do is, something that will certainly benefit the project, but you'll have to ask for permissions, and it's not easy to convince others, or it takes too much time. The book recommends that in such case you should think of the simplest thing you can ask for and you won't get rejected, after that it's okay to try whetting others' appetite by showing them a 'glimpse of the future', basically saying 'Of course it would be nicer if we add add this or that feature', but pretend it's not that important and wait, there is a good change they would tell you to implement it.

🗨 This is a general social skill I someone taught me, that is, not trying too hard to offer what you have if the other part doesn't seem to care, like when you want to advise someone who doesn't seem to care, sometimes talking too much doesn't help and makes your words less meaningful, this is clearly true for school teachers for instance, the teacher's words might lose impact if they repeat it too many times. Sometimes silence could intrigue the student because it's different and makes them want to hear from you.

Tip 6: Be a Catalyst for Change

The book brings up the famous Boiled Frogs story, that if you throw a frog in some hot water, it will jump immediately, but if you gradually heat the water, it won't notice. That's not what happens in real life, but it's the moral of the story is worth noting.

Tip 7: Remember the Big Picture

You need to know what's going on around you in the project and in life in general. You need to understand the big picture.
The book even recommends that you develop situational awareness and observation skills; for instance, close your eyes. - well you can't read like that - but try to count the number of light bulbs in the room you're in, the number of people in the room, etc. It's a good idea to develop this skill and sharpen your mind for details, and do the same for your projects.

5. Good-Enough Software

You should know what the minimum quality required for the project, you can spend a lot of time perfecting parts of the system, but don't overdo it. It depends on the kind of software you're working on, but in most cases, releasing 'good enough' software
But you need to define what's 'good enough' for your project; it surely doesn't mean low-quality code and neglecting important things like security.

Tip 8: Make Quality a Requirements Issue

6. Your Knowledge Portfolio

- Tech changes a lot, and you need a strategy for coping.
- Your knowledge portfolio encompasses many things, including all of your experiences, domain knowledge, CS knowledge, etc.
- You should invest in your knowledge portfolio.
  The hard part is forming a habit of learning and expanding your knowledge portfolio. But it's very rewarding as you'll be learning so much without even thinking about it.
- You should create a habit, even if you do a little bit every day, because what matters more in the long term is the habit you're building, not what you're learning.
- Variety matters; the more different the things you know, the better. You certainly must master at least one technology, but you should absolutely learn different technologies.
- It's risky but very rewarding to learn an emerging technology.

Tip 9: Invest Regularly in Your Knowledge Portfolio

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

7. Communicate

Tip 11: English is Just Another Programming Language

i.e. you got to master it too!

The book is basically saying, you're going to work with people, so it's important that you learn some communication skills (so-called 'soft skills' that are actually hard to learn)

🗨 Did the book just mention Neuro Linguistic Programming ?! It's a known pseudoscientific approach for communication skills and psychotherapy. The advice in this section is turning into self-help stuff.

The book gives some communication tips that feel generic but do not mean it's devoid of some truth in them: know your audience, know what you want to say, involve the audience, be a listener, make documents look good, and so on…

🗨 Speaking of making documents look good, I've been using Typst for the last year, and it's been great. I like it more than LaTeX[^latex]; it's great for writing pretty much all types of documents.

Tip 12: It's Both What You Say and The Way You Say It

Tip 13: Build Documentation, Don't Bolt It On

- Don't add documentation as an afterthought; it should be part of your workflow.
- Add comments to modules and exported functions to help the other devs understand how to use them.
- You don't have to add comments to every single function; that would make things harder to maintain because now you have to modify code and make sure the comments are consistent. Focus on commenting the API[^api], i.e., things other devs will use. For other things, explain the why behind your approaches. The code already explains how it's done.

## Chapter 2: A Pragmatic Philosophy

## Footnotes

[^think]: It's worth noting that this is not at odds with trying things out when you're trying to understand the problem; sometimes it's a good idea to start getting your hands dirty and start with some code, or come up with examples when you're trying to solve a math problem. The problem is when you start to get into autopilot mode and enter what I like to call the WHEEL loop (write, hope, execute, errors, loop)

[^latex]: Pronounced as /latek/

[^api]: This term is used in many different contexts; it's not just about web APIs; it could mean a bunch of library functions that you can use without needing to think about how they work inside. You just need to understand the expected inputs and outputs.
