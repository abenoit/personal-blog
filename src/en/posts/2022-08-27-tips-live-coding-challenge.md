---
title: Live coding challenge tips
description:
date: "2022-08-27"
tags: [tech, challenge, job]
image: "/images/live-coding-challenge/computer-girl.jpg"
translationKey: "post_live_coding_challenge_tips"
---

Let's continue the interview tips series with the dreaded **live coding challenges**! Personally, I have a knot in my stomach by simply reading the email that tells me that I have a live coding session in a recruitment process (and I've been dev for 10 years).

Applying for a job in tech usually comes with its set of technical tests. Live coding, deep dive, MCQ... each type of interview has its own set of advantages and disadvantages.

I've had both hats, but now I'm more of the interviewer. I wanted to share here the advice that can help you if you are going to have tech challenges to pass.

> That does not mean that by following these tips, you will necessarily succeed in your interview!

I'm going to provide you keys to having a clearer, cleaner and more organized approach, which are qualities generally sought after by the people who will interview you. Obviously, the technical level and other qualities expected depend on the company and the position you are applying for. In any case, these tips are essential elements that can only work in your favor. Or even potentially play against you if they are not or not well presented.

# Live coding challenge tips

## What's a live coding challenge

The goal is to solve one (or more) tech exercises **live** in front of one or several people. This kind of test is difficult and particularly dreaded because **we find ourselves naked in front of one or more strangers** who judge us in real time, which leaves little room for error. Anyway, that's what we say to ourselves.

## A two-way test

As with any interview, the goal must always remain the same: **make the person in front of you want to work with you.**. But this time it goes both ways; it is also necessary that the people in front of you make you want to work with them - finding yourself in front of a pretentious \*\*\* probably remove all desire to join their company!

My tip is then to approach this interview as an exchange, a discussion or even as a mob-programming session. It may be your future colleagues that you meet for the first time. These people in front are not mere spectators, they are here to accompany you, answer your questions, unblock you if necessary.

### Before the interview: the preparation

As with any interview, it is best to do your research beforehand and prepare questions. In addition to giving context, it allows you to have questions to ask at the end of the interview. You can then search conferences, technical blogs, publications... It is not only important to show your interest in the company, but also and above all to show that you are planning.

Regarding the technical part, the process is sometimes communicated in advance, which then makes it relatively easy to know what to work on. If not, several possibilities and resources:

- the company is well-known: [Glassdoor](https://www.glassdoor.fr/) lists interview testimonials from candidates who can then give an indication of the type of exercise usually given.
- if nothing appears on GlassDoor, it is always possible to train for free on platforms like [CodingGame](https://www.codingame.com/) on more or less complex exercises.

## During the interview

### Instructions

It seems extremely basic as advice, but it is nevertheless the most important. **Read the instructions, make sure you understand them. and LISTEN.** If there is any doubt about an instruction, ask questions. It is better to repeat than to be wide of the mark. A smarter way to make sure that you have understood correctly (or precisely that you are not sure you understand) is to reformulate the exercise in your own words, and ask if this is what is expected.

## Show our best self

The most common syndrome I've noticed among developers is **over-engineering**.

> "Super easy, I know how to do it, so let's go for a nested double reduce!"

Expectation VS Reality: We forget the return, the parameters are in the wrong direction, we initialized the function badly and we made a typo for each word.

With stress, it's actually super hard to output code to an editor you're probably not familiar with - probably without auto-completion, and with people watching and you think are judging every typo. Even when we are used to it. Even when you're a senior!

<mark>Overall, and especially when stressed, #1 tip: ITERATE.</mark>

```
Example: start with a first `for` loop, mutated variables here and there. Then extract into a function. Then use a `.map` instead (or why not a `reduce` if you really feel like it). etc
```

<mark>And the secret that isn't one - tip #2 TALK.</mark>

Super important to avoid isolating yourself in your exercise and to make your intention understood by the people in front. They will be able to understand, help or challenge you. **You give yourself a chance to argue your choices while showing that you are objective about your code.**

```
Example: "Here I'm going with a naive approach to start with, it's not ideal performance-wise, but I'll come back to it later."
```

And if the result is not as expected, **de-dramatize**. The interviewers know that it is a stressful exercise and that no one is in possession of all their means.

## Manage stress

On D-Day, whether you've been preparing for weeks or not at all, you're usually **hyper-stressed** (except superhuman people, of which I'll never be one).

Stress is actually pretty good **in small doses**. It allows you to be concentrated, to try to surpass yourself during the exercise. But it is essential not to be overwhelmed. Several techniques exist:

- To know oneself
- Preparing for the interview
- To ask questions

### Know oneself

It is difficult to know our reactions given a situation before being actually confronted with it. In a stressful situation in front of people, do I tend to block / make jokes / talk too much...?

It is often after several interviews that we get to know oneself other better, through what we feel but also through the feedback that we can receive (or ask to receive) after the interview.

## Ask questions & speak

Ask questions by bouncing on the test or remarks of the speakers; "are you using a /lib/archi/process?etc convention". This shows that you care and can give you insight into how the teams are working.

If possible, practice **speaking while coding**. We rarely have this need on a daily basis, so it's quite unnatural and probably destabilizing at first. At least raise your head between a few lines of code to explain what you're trying to do. **Ask for help if you are stuck.**

The important thing is to keep in touch with the interviewers. Yes it's a technical test but the fact remains that an important part of the success of this challenge is attributed to communication and feeling because it is an essential component in our daily life (even for the devs yes).

## At the end of the interview

This is the perfect time to say what you thought of the test and your performance. The ideal is to provide suggestions for improvements to the rendered code, whether technical, functional, from a QA point of view, performance, etc.

<mark>No code is perfect (and certainly not code from a live coding challenge). Tip #3: stay objective and humble!</mark>

# Conclusion

Live coding challenges are difficult and stressful, it's normal to feel that way. The interviewers - our future colleagues? - are here to help us and put us at ease. Count on them, but help them by keeping communication open all the time.
