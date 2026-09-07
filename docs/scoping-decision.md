# Scoping Decision — Progressive Overload Tracker


**Author:** Allie Moldenhauer ·  **Date:** 2026-09-06  ·  **Course week:** 2

---

## 1. Problem

For regular gym-goers who want to use a progressive overload workout plan to build strength over time. Several of these weightlifters resort to using the notes app on their phone or a physical notebook to track their workouts and manually calculate future weights, reps and sets for workouts. With tracking, calculating and planning out workouts in the notes app, users are likely to make mistakes and cannot easily utilize the bulk of their previous workout tracking, as there is no system to automatically consolidate their previous workouts. An application that allows users to track, plan and automatically calculate future workout goals would allow these weightlifers to more easily track, see progress and plan out their workouts. 

## 2. Evidence a user exists

Interviewed KM/weightlifter on 2026-09-04, 35 minutes, past-tense questions only.
Full write-up in `docs/interviews/2026-09-04-KM.md`.

- "The most annoying part of using my notes app is not having a reliable place to check on my phone."
- "I don't spend money on any solutions I'm not 100% sure work."
- "I would consider looking into an app that tracked my progress over time."

## 3. Chosen scope — Must features

| # | Feature | Hours |
|---|---|---:|
| 1 | Ability to put in and save workout plan in the application | 6 |
| 2 | Store data from recorded workouts and workout plans | 4 |
| 3 | Create chart/graph to display progress over time for different exercises | 8 |
| 4 | Set workout times on a calender built into the app | 8 |
| 5 | Suggest future goals based on previous workout performance | 6 |
| 6 | Able to input workouts as you complete them in the gym | 6 |
| | **Feature total** | 38 |
| | Walking skeleton + continuous integration | 12 |
| | Deployment + clean-machine test | 8 |
| | **Construction total** | 60 |

Plan: 60 hours. Hard ceiling: 75. My number: 60. There is some slack, but it would steal from testing, so staying under the 60 hours is important to make sure that I have enough time to make sure that the application actually works and I end up with a functioning product. 

## 4. Should features — built only if there is room

Currently no "should" features - will bump features here if the scope appears to become unreasonable in future weeks. 

## 5. Out of scope — will not be built

Suggested workout plans, either by AI or built-in suggestions.
Meal planning or nutrition guidance.
AI coaching assistant for workout advice.
Pre-planned workouts to follow.
Ability to export workout plans/workout data from the app.
User accounts - assume user is already logged in for the purposes of this capstone.
AI-assisted planning for future workout/workout targets.
Integrated web version or available on multiple platforms - building only to run on Android.


## 6. Accepted tradeoffs

Rejected using AI-assisted suggestions for future workouts or using AI to determine future workout numbers. I believe that this feature would take too long to integrate and is not necessary for the application to achieve it's purpose. If I either finish more quickly than expected or continue to build on this project in the future, I may revisit this feature as a possibility. 

## 7. Rejected candidates

**Rejected: Starbucks IMs.** Dependencies cannot be verified - no public access exists for the database that I would need to complete the project. 

**Rejected: CleanTrack.** Cannot deploy on actual company devices for testing, only on my personal device. 

| Dependency | Candidate | Exercised | Result | Key? | Rate limit | Terms read |
|---|---|---|---|---|---|---:|
| Inventory Database API | B | researched | UNVERIFIED - no public endpoint available | unknown | unknown | - |

## 8. Hour budget, reconciled

| Weeks | Phase | Hours |
|---|---|---:|
| 1–2 | Inception | 30 |
| 3–4 | Requirements | 30 |
| 5–6 | Design | 30 |
| 7 | Planning | 15 |
| 8 | Design review + midterm | 15 |
| 9–12 | Construction + verification | 60 |
| 13 | Documentation | 15 |
| 14 | Deployment + handoff | 15 |
| 15–16 | Presentation + delivery | 30 |
| | **Total** | **240** |

My project does fit within the 60 hours budget, cutting any AI-assitant features in order to fit inside this budget. 

Compared to 240 Hour Scope Sizer: Sizer states that the project will most likely fit in with an estimated total hours of 224 +/-34%

## 9. The one hard part

Building an algorithm that can take information from previous workouts and take that information in order to determine future workout targets. Including research on how to mathematically and algorithmically track progressive overload and pulling past performance from the database in order to determine those goals will make the determining of future goals the hardest part of this project. 

## 10. Risks and the scope-cut trigger

| Risk | Likelihood | What it costs me | Early warning sign |
|---|---|---|---|
|  My work schedule is variable. Time I block off for this class during this week could get taken up by my future work schedule.  | M | Possibility of lost time or scheduled time for blocks being lost, could ultimately cause me to fall behind | Schedule posted two weeks in advance |
| Two 8-week classes will wrap up in Week 8 and will likely require more dedicated time during the last week than usual. | H | Lost time in Week 8 for the project due to my other courses |  Can look ahead, will have a better idea by week 6/7 what final week will entail. |
| I have a tendency to become overambitious when building projects and bite off more than I can chew. | M | Time lost to unneccesary features or time lost because I refuse to settle for a simpler version | Struggling to get a walking skeleton together by Week 9 of the project |

**Scope-cut trigger.** If I am behind in my estimated budgeted hours by more than 8 hours by the end of Week 11, I will cut
the future suggested goals feature first, then the calendar for when workouts are planned by day/week, then a graph to display workout progress over time. Decided now, in advance, so I do not have to decide
it while panicking.

---

**Signed:** Allie Moldenhauer, 2026-09-06
**AI use for this document:** No AI usage in the creation of this document. 
