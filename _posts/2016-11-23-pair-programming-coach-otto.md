---
layout: post
title:  PP Coaching at otto.de, First Code, Then Process
date:   2016-11-23
categories: engineering
---

My highlight session at [XP Days 16](http://www.xpdays.de/2016/) that really gave me new impulses was "Pair Programming – Developers' Friend, Managers' Enemy?" by [Stephan Kraus](https://www.otto.de/unternehmen/jobs/interviews/interview-Stephan-Kraus.php) and [Thomas Much](http://www.muchsoft.com/) about Pair Programming Coaching at [otto.de](https://www.otto.de). In a nutshell, Thomas worked as developer/coach in a team for 2 sprints, in order to foster Pair Programming and other Agile Engineering Practices, bringing the team's engineering capabilities sustainably to the next level.

The motivation to use this intense coaching method was to:

  * Keep knowledge distribution high
  * Keep quality and maintainability high
  * Prevent team erosion - teams that perform, but get stuck in a rut and do not improve anymore erode over time, either in their quality or people really leave

Regarding knowledge distribution, static analysis showed that some of the parts of the platform, that were of high complexity, were only ever touched by one or two developers. This kind of knowledge islands are super dangerous for a team and company.

## Method: A coach pairs inside the team for 2 sprints

The basic idea to solve these problems was as follows: Encourage teams to use a communication-intensive Agile Engineering practice (Pair Programming). The goal was to reap benefits in this direction:

  * Increase quality through continuous, implicit reviews (making code review superfluous)
  * Create more readable code, especially when juniors and seniors pair with each other
  * Improve the general team spirit through tighter day-to-day collaboration

The concrete method was a coach working in a team as a developer, contributing to the sprint goal for 2 sprints. The twist would be (obviously) that the coach does not have an own workstation and can only contribute to the team by pairing. The coach focuses of course on delivering value to the team, but also on fostering new and enhancing existing Pairing (and general coding) Practices in the team, by asking developers for feedback, reflection and suggestions for improvement. This is a high investment, but as Stephan Kraus said "Pair Programming really pays off in the long term".

What was new for me: This method focuses on improving a team's *code* first, then their process. The reason is in most developer's central motivation to be software developers: "Let us write great code together". Think of an architect working with masons, who are only able to build brittle and skewed walls. Likewise, if a team can not derive pride from their main activity, because they can not produce great code, they will struggle with their process as well. I would have doubted this reasoning before, but apparently it worked out for Thomas and Stephan.

## Everyone has to try, and taking breaks needs to be learned

Thomas and Stephan were so kind to also provide us with some details, that made their case much more credible:

  * This coaching took place during the hot relaunch phase of otto.de. I think this is important to the developers that were paired with, because if more pairing does not slow you down in a critical phase, there is no reason to stop it in any other phase
  * Before working in each team there was a kickoff workshop with the team to collect and set expectations and give Thomas an idea what the focus will be
  * Pairing was of course voluntarily for everyone, but Thomas used the same motto as I for my daughter regarding vegetables: "You have to try at least once."
  * There was a Retrospective meeting on the Pairing practice after 1 Sprint, to gather improvements and if need be to pause the pairing coaching
  * Feedback was continually provided throughout the Sprint
  * Thomas did not have an own workstation, this created a slight, but healthy social pressure for the developers to actually pair with him

## Hints & Pitfalls for Pairing

Thomas also provided some useful strategies when actually pairing like this:

  * Change Roles (Driver + Navigator) frequently, TDD may help with that
  * Change pairs frequently, every 2-4h to avoid fatigue
  * Choose only tasks that are suitable for pairing (sliced suitably small <1 day, with stories that are smaller than one sprint)
  * *Breaks* were the most important thing and had to be practiced explicitly. The Pomodoro technique might help here

What I liked was that Thomas and Stephan also included some pitfalls they ran into, as not everything works out perfectly ever:

  * Pairing is not always pairing: If in a team only the same pairs form all the time, you do not reach the goal of broad knowledge transfer
  * Very good engineers needs someone on their level to really benefit from pairing (this can be the coach or a co-worker), otherwise it is more of a mentoring session
  * Less confident engineers need encouragement to show that they have a lot of strengths thattef are valuable in a pairing session

## Conclusion 

This method sounds like a viable way to improve engineering practices in agile teams. Even those that already practice e.g. pair programming received new insights from working with Thomas and reflecting on their practices. 
Open questions for me are, how well you can foster more Agile Engineering Practices (Refactoring, Clean Code, TDD, ...) and what to do different with them. 
What I really like about this approach that it sounds much more sustainable than for example Team Dojos. In my opinion these always hold the danger of simply withering away after a while. In the mode presented by Thomas and Stephan however, there is no gap from pairing-in-katas to pairing-on-real-code that teams have to jump across.

So, time to try pair programming coaching out!