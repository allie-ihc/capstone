# Idea Canvas — Candidate C

**Candidate name:** CleanTrack
**Date started:** 2026-09-01   **Well it came from:** <work>

---

## 1. Problem statement

For              workers and managers at a Starbucks who need to keep track of cleaning tasks in their store
who              do not have access to an easy-to-utilize system for tracking when cleaning is completed
the problem is   cleaninng tasks get missed, performed wrong or mistakenly marked off because the current solution is hard to understand
which costs      3-5 missed cleaning tasks a week; 4-6 miscommunicated either completed/not completed tasks per week
Today they       track cleaning tasks on paper, using a book that lists each task that needs to be completed every week
which falls short because  explanations of tasks are unclear, monthly tasks are thrown in with weeky tasks creating a lack of clarity about when to perform each task, requires looking back through tracked data in order to determine what needs to be completed. 

> If the `which costs` line has no number in it, stop and go get one.

## 2. Evidence a user exists

- **Person spoken to:** <initials or role — not "people in general">
- **Date and length:** <YYYY-MM-DD, minutes>
- **Three verbatim quotes:**
  1. "<exactly what they said>"
  2. "<exactly what they said>"
  3. "<exactly what they said>"
- **The workaround they already use:** <...>
- **Full write-up:** `docs/interviews/<YYYY-MM-DD>-<initials>.md`

## 3. Candidate scope (Must features only)

| # | Feature (one vertical slice each) | Hours |
|---|---|---:|
| 1 | Mark off tasks completed with name/date attached | 5 |
| 2 | Create custom tasks/update current tasks | 6 |
| 3 | Check history for each task, including when it was completed, when and by who | 8 |
| 4 | Create links for each task that lead to the explanation for how to complete | 8 |
| 5 | List tasks to be complete for each week, including bi-weekly and monthly tasks added when they need to be completed again | 10 |
| | Walking skeleton + CI | 12 |
| | Deployment + clean-machine test | 8 |
| | **Construction total** | 57 |

Budget: plan on **60 hours**, hard ceiling **75**. Above 75 you are borrowing from
testing and documentation, which are graded.

Compared to 240 Hour Scope Sizer: Range fits within the 240 hours budget with room to spare. 

## 4. Out of scope — will NOT be built

1. In-app explanations - link to where explanation for each task already exists
2. Accesible on multiple platforms - built to run on mobile only, easiest for tracking
3. Automatically update for new equipment
4. Customized lists based on needs of different stores - allow for customization instead
5. AI explanations or chatbots for how to complete tasks
6. Prioritization levels for different tasks
7. Deleting data after a certain period of time - for purposes/constraints of this project, will keep everything
8. Tracking what an individual person has done by the person - track only task completed w/ person attached instead

## 5. Feasibility screen

| Gate | Verdict | Evidence (dated) |
|---|---|---|
| **Build** — novelty load ≤ 2 | pass / fail | <technology list, each marked known/new> |
| Development IDE | pass | Swift - new |
| **Get** — every dependency exercised for real | pass / fail | <status code, saved response, date> |
| **Ship** — a named deployment target, terms read | pass / fail | <target + pricing page read on YYYY-MM-DD> |
| iOS 26 | pass | can deploy on my personal device for demonstration purposes |
| **Show** — a stranger sees it work in 10 minutes | pass / fail | <the ten steps, written down> |
| Demonstrate all features of the application | pass | 1. Open up task list for the week, 2. Mark of tasks with name of person completing them, 3. Go back and demonstrate that task is removed from the list, 4. Navigate to future weeks to display bi-weekly/monthly tasks, 5. Demonstrate that future tasks cannot be marked off until that week, 6. Navigate to previous week and show tasks marked off with times/dates and person who completed them, 7. Demonstrate that past tasks cannot be marked off, 8. Create a new custom task w/ duration, 9. Edit a currently existing task, 10. Delete a task from the list |

**Technologies:** Swift - new
**Novelty load:** 1

## 6. The one hard part

Having the application build schedules of cleaning tasks for each week based on the frequency that each task needs to be completed will be the hardest part of this project. Algorithmically determining and buiding schedules with tasks that need to be completed over different times will require a complicated algorithm and therefore will be the hardest part of this project. 

## 7. Scorecard (1–5 each; weight in parentheses)

| Criterion | (w) | Score | Weighted |
|---|---:|---:|---:|
| Evidence a user exists | 3 | 3 | 9 |
| Fits ~45 hours of features | 3 | 5 | 15 |
| Novelty load | 2 | 5 | 10 |
| Dependencies verified | 2 | 5 | 10 |
| Demonstrable in ten minutes | 1 | 5 | 5 |
| **Total (max 55)** | 49 | | |

## 8. If this candidate is rejected

I certainly think that this project would be beneficial, but I do think that based on the nature of the application, I wouldn't be able to properly test it within the timeframe I have for this capstone. Since this application is meant to be used over weeks and months for a store and I only have a few weeks for this project that I can actually test the application, I believe that it would be better to defer this project to a later date rather than build it now. In addition, I do not believe that I would be able to deploy it to actual company devices, so a true test of the software would be unavailable to me. 