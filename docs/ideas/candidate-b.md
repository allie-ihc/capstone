# Idea Canvas — Candidate B

**Candidate name:** Starbucks IMS
**Date started:** 2026-09-01   **Well it came from:** work

---

## 1. Problem statement

For              shift and general managers at Starbucks
who              struggle looking through complicated menus and options to complete inventory related tasks with the current system
the problem is   different naming conventions, complicated applications and non-standardized way of tracking inventory across different applications creates errors and difficultly completing inventory-related tasks
which costs      (in the Grafton store, for example): 5% of food expiring before being sold every week, running out of 3-5 products every week
Today they       use currently available applications as well as spreadsheets and tracking or counting inventory on paper
which falls short because  complex or non-integrated systems lead to greater human error; product is miscounted, the wrong amount of product is ordered and product either expires before it can be used or product runs out long before the next order comes

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
| 1 | Markout expired/donated items | 4 |
| 2 | Count items on-hand twice a week | 6 |
| 3 | For counted items that are significantly higher/lower than current database estimate, push high variance count | 8 |
| 4 | Place orders with estimates for products based on on-hand and ordered items and expected demand | 10 |
| 5 | Create custom orders for specific products manually | 6 |
| 6 | Tranfer product from or to different stores manually | 6 |
| 7 | Look up and adjust receipts for recently delivered orders | 8 |
| 8 | Look up future orders, including items and amounts ordered | 7 |
| | Walking skeleton + CI | 12 |
| | Deployment + clean-machine test | 8 |
| | **Construction total** | 75 |

Budget: plan on **60 hours**, hard ceiling **75**. Above 75 you are borrowing from
testing and documentation, which are graded.

Compared to 240 Budget Scope Sizer: Project will likely run 17 hours over, fits but with little wiggle room. 

## 4. Out of scope — will NOT be built

1. AI-assisted inventory counting/tracking
2. AI-assisted estimates to create orders
3. Calculated store waste based off of orders and counts
4. Ability to use on multiple platforms - build to run on one machine that I can test
5. Update from the app to include/get rid of products
6. Analyze and compare store metrics against other stores
7. Track expiration dates of items
8. Central database where products are stored - rely on infrastructure that already exists

## 5. Feasibility screen

| Gate | Verdict | Evidence (dated) |
|---|---|---|
| **Build** — novelty load ≤ 2 | pass / fail | <technology list, each marked known/new> |
| Development IDE | pass | Visual Studio Code |
| **Get** — every dependency exercised for real | pass / fail | <status code, saved response, date> |
| Inventory API | fail | not publicly accessible |
| **Ship** — a named deployment target, terms read | pass / fail | <target + pricing page read on YYYY-MM-DD> |
| Windows 11 | pass | can deploy for free on a clean VM |
| **Show** — a stranger sees it work in 10 minutes | pass / fail | <the ten steps, written down> |
| Navigate through application | pass | 1. Boot up application, 2. Create an order, 3. Place that order, 4. Go back and demonstrate that order is saved and accessible in-app, 5. Navigate to order receipt, 6. Change number of items on receipt, 7. Save changed receipt, 8. Navigate to counts, 9. Enter data for count, 10. Submit count |

**Technologies:** <name> (known/new) · <name> (known/new) · <name> (known/new)
**Novelty load:** <count of "new">

## 6. The one hard part

Working with a database that I have not been introduced to and that I cannot change because other systems are already dependent on. Taking a database and API system that already exists and having to build on top of it to complete a number of tasks will be the hardest part of this project. 

## 7. Scorecard (1–5 each; weight in parentheses)

| Criterion | (w) | Score | Weighted |
|---|---:|---:|---:|
| Evidence a user exists | 3 | 2 | 6 |
| Fits ~45 hours of features | 3 | 3 | 9 |
| Novelty load | 2 | 5 | 10 |
| Dependencies verified | 2 | 1 | 0|
| Demonstrable in ten minutes | 1 | 5 | 5 |
| **Total (max 55)** | 30 | | |

## 8. If this candidate is rejected

While I still think that this would be a beneficial application to create, without public access to the inventory system I do not believe that this is a project that I am able to complete. While I could build a mock database for testing my application, I wouldn't have access to the shape of the actual database which would mean that my application would not be able to achieve it's intended purpose of connecting into the actual database and creating a better front end for the database. In addition, the features would take up a high amount of the budgeted time and would exceed the ideal 60 hours of development time, meaning that this project likely falls outside of the scope that I have for this project and is potentially deferred to a later date. 