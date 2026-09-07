# Idea Canvas — Candidate A

**Candidate name:** Progressive Overload Tracker
**Date started:** 2026-09-01  **Well it came from:** hobby

---

## 1. Problem statement

For              regular gym-goer who weightlifts and uses a progressive overload system to increase strength over time
who              has no easy system to plan, track and calculate progress in weightlifting over time
the problem is   no simple way to track workouts and plan out future workout plans over time
which costs      1-2 errors per week in tracked workouts; extra 10 minutes before each workout to set up tracking/calculate weights for each exercise
Today they       use their notes app to track workouts and manually calculate new weight numbers for future workouts>
which falls short because  <the specific reason the workaround fails

> If the `which costs` line has no number in it, stop and go get one.

## 2. Evidence a user exists

- **Person spoken to:** <KM>
- **Date and length:** <2026-09-04, 30>
- **Three verbatim quotes:**
  1. "The most annoying part of using my notes app is not having a reliable place to check on my phone."
  2. "I don't spend money on any solutions I'm not 100% sure work."
  3. "I would consider looking into an app that tracked my progress over time."
- **The workaround they already use:** notes app to keep track of and plan future workouts, using knowledge from previous classes and independent research
- **Full write-up:** `docs/interviews/2026-09-04-KM.md`

## 3. Candidate scope (Must features only)

| # | Feature (one vertical slice each) | Hours |
|---|---|---:|
| 1 | Ability to put in and save workout plan in the application | 6 |
| 2 | Store data from recorded workouts and workout plans | 4 |
| 3 | Create chart/graph to display progress over time for different exercises | 8 |
| 4 | Set workout times on a calender built into the app | 8 |
| 5 | Suggest future goals based on previous workout performance | 6 |
| 6 | Able to input workouts as you complete them in the gym | 6 |
| | Walking skeleton + CI | 12 |
| | Deployment + clean-machine test | 8 |
| | **Construction total** | 60 |

Budget: plan on **60 hours**, hard ceiling **75**. Above 75 you are borrowing from
testing and documentation, which are graded.

Compared to 240 Hour Scope Sizer: Sizer states that the project will most likely fit in with an estimated total hours of 224 +/-34%

## 4. Out of scope — will NOT be built

1. Suggested workout plans, either by AI or built-in suggestions
2. Meal planning or nutrition guidance
3. AI coaching assistant for workout advice
4. Pre-planned workouts to follow
5. Ability to export workout plans/workout data from the app
6. User accounts - assume user is already logged in for the purposes of this capstone
7. AI-assisted planning for future workout/workout targets
8. Integrated web version or available on multiple platforms - building only to run on Android

## 5. Feasibility screen

| Gate | Verdict | Evidence (dated) |
|---|---|---|
| **Build** — novelty load ≤ 2 | pass / fail | <technology list, each marked known/new> |
| Android Development IDE | pass | Android Studio - new |
| Local database | pass | SQLite - new |
| **Get** — every dependency exercised for real | pass / fail | <status code, saved response, date> |
| No dependencies necessary | pass | determined 09-06-2026 |
| **Ship** — a named deployment target, terms read | pass / fail | <target + pricing page read on YYYY-MM-DD> |
| Android phone running Android 16, terms read | pass | free to deploy, read on 09-06-2026
| **Show** — a stranger sees it work in 10 minutes | pass / fail | <the ten steps, written down> |
| Deploy and boot up on Android phone | pass | 1. Deploy on Android device, 2. Open app, 3. Open to create a new workout plan, 4. Set a date to complete that workout plan, 5. Access workout plan and begin a workout, 6. Put in information for that workout, 7. Demonstrate that the information is stored in the workout history, 8. Navigate to displayed past workout information by exercise, 9. Demonstrate future goals suggested for workouts | 

**Technologies:** Android Studio - new · SQLite - new 
**Novelty load:** 2

## 6. The one hard part

Building an algorithm that can take information from previous workouts and take that information in order to determine future workout targets. Including research on how to mathematically and algorithmically track progressive overload and pulling past performance from the database in order to determine those goals will make the determining of future goals the hardest part of this project. 

## 7. Scorecard (1–5 each; weight in parentheses)

| Criterion | (w) | Score | Weighted |
|---|---:|---:|---:|
| Evidence a user exists | 3 | | |
| Fits ~45 hours of features | 3 | | |
| Novelty load | 2 | | |
| Dependencies verified | 2 | | |
| Demonstrable in ten minutes | 1 | | |
| **Total (max 55)** | | | |

## 8. If this candidate is rejected

<Write the rejection paragraph NOW, while you still like the idea. Name the gate it
failed, the number that killed it, and the condition under which you would revisit
it — or say plainly that it is closed, not deferred.>