# 📝 MY_WORK: Student Information, Development Log, Reflection & Answers

> This is the **only file** your instructor reads to grade Parts 3 and 4 (documentation and video). Everything you write here must be **in your own words**.

> **DRAFT — review and personalize before submission.** The reflection paragraphs are example wording based on the supplied source code, not statements verified about my own feelings or study process. Replace each `TODO` with true details and add the original starter output and video link. Keep the instructor section headings unchanged.

---

## 🛑 STOP: Read This Before You Do Anything Else

> ### 1️⃣ Read the whole `README.md` first
> The `README.md` in this repository contains the full instructions: how this assignment continues Assignment 1, the Chapter 5 recap, class descriptions, feature specifications, question prompts and the video script. **If you skip it, you will lose marks.**
>
> ### 2️⃣ Understand the full code before answering any question
> Open `SchedulerSimulationSync.java` and read it **from top to bottom**. You must be able to explain what `SharedStats`, `ReadyQueue`, `CpuWorker`, `RaceWindow.pause()`, `ReentrantLock` and `Semaphore` do **before** you write a single answer in Parts B and C. **Run the original starter first** (it is intentionally broken) and **save its output**: you need it for Question 1 of Part C.
>
> ### 3️⃣ Use only the code of this repository
> Work **only** on `SchedulerSimulationSync.java` from this repository. Do **not** copy or paste code from your previous assignments.
>
> ### 4️⃣ Commit many times, not once
> A single commit, or all commits made in the last hour, costs you **-0.5 mark**. See the [Commit Rules](#-commit-rules-mandatory) below.

**How to use this file:**
1. Fill in your **Student Information** (below) right now.
2. Follow the steps in the **Work Roadmap** in order.
3. Update the **Development Log** *every time* you work on the assignment, not at the end.
4. Do not delete any section header. Replace the `[...]` placeholders with your own text.

---

## 👤 Student Information

> ⚠️ **WARNING:** Fill this in first. Your name and ID must match the student ID you set in `SchedulerSimulationSync.java` (line 304) and the one you say in your video.

| Field | Your Answer |
|-------|-------------|
| **Full Name** | Fatima ibrahim zaid alruziqi |
| **Student ID** | 445052065 |
| **University Email** | 445052065@std.psau.edu.sa |
| **GitHub Username** | Fatima-1209 |
| **Repository Link** | https://github.com/Fatima-1209/OS-Assignment3-Fatima-Altmimi |
 
---

## 🎥 Video Link

**Video Link**: **TODO — paste the real public video URL after uploading `[445052065_Assignment3_Demo.mp4](https://drive.google.com/file/d/1o5PHrgWp0Hawai8JF8fUs9AOkxfUfNM-/view?usp=drive_link)`.**

> ⚠️ **WARNING:** The video must be **publicly accessible** ("Anyone with the link can view") on **Google Drive**, **YouTube (Unlisted or Public)** or any other cloud file-sharing system. A private, restricted or broken link counts as a **missing video (-1 mark)**.
>
> 💡 **TIP:** Open the link in a **private/incognito window** before you submit. If it asks you to log in or request access, it is not public.
>
> 📌 **NOTE:** The link goes in **this file only** (`MY_WORK.md`), **not** in `README.md`. Name your video file `StudentID_Assignment3_Demo.mp4`. It must last **2 to 3 minutes**.

---

## 🗺️ Work Roadmap (follow in this order)

| Step | What to do | Where | Marks |
|:----:|------------|-------|:-----:|
| 0 | Read `README.md`, read the full code, **run the original starter and save its output** (it fails on purpose) | Your IDE | – |
| 1 | Fork, rename, keep the repo **PUBLIC**, set your student ID (line 304), **commit** | GitHub + code | Part 1 (1) |
| 2 | Feature 1: Mutex lock on the ready queue, **commit** | Code | Part 2 (0.25) |
| 3 | Feature 2: Mutex lock(s) on the shared statistics, **commit** | Code | Part 2 (0.25) |
| 4 | Feature 3: Counting semaphore instead of busy waiting, **commit** | Code | Part 2 (0.5) |
| 5 | Development Log (5+ entries, different dates) | This file, Part A | Part 3 (0.5) |
| 6 | Reflection (4 questions) | This file, Part B | Part 3 (0.5) |
| 7 | Technical Answers (4 questions) | This file, Part C | Part 3 (0.5) |
| 8 | Record the video, upload it, paste the link above | Video + this file | Part 4 (1.5) |
| 9 | Final check, then submit the repo link on Blackboard | Blackboard | – |

> 💡 **TIP:** Tick each step off as you go. Do not leave the log, the reflection or the video for the last day.

---

## 🔁 Commit Rules (MANDATORY)

> ### ⚠️ MANY COMMITS ARE REQUIRED. A single bulk commit is penalized (-0.5 mark).

**Minimum: 4 meaningful commits. Aim for 7 or more.**

| # | Commit | Example message |
|:-:|--------|-----------------|
| 1 | Student ID set | `Set my student ID: 441234567` |
| 2 | Feature 1: Ready queue lock | `Feature 1: Protected the ready queue with a ReentrantLock` |
| 3 | Feature 2: Statistics locks | `Feature 2: Added locks to the shared statistics counters` |
| 4 | Feature 3: Semaphore | `Feature 3: Replaced busy waiting with a counting semaphore` |
| 5 | Development log entries | `Docs: Added development log entries 1-3` |
| 6 | Reflection and answers | `Docs: Completed reflection and technical answers` |
| 7 | Video link | `Docs: Added demo video link` |

**Rules:**
- ✅ **One commit per feature.** Do not put all three features in one commit.
- ✅ **Commit after each work session**, and after each part of this file.
- ✅ **Spread your commits over different dates.** Not all in one day.
- ❌ **Do not make all commits in the last hour** before the deadline (November 14, 2026).
- ❌ **No vague messages** like `done`, `update` or `final version`.

> 💡 **TIP:** Your commit history is checked and you **show it in your video** (at least 4 commits visible). Your development log dates should match your commit dates.
>
> 💡 **TIP:** **Use VS Code** (see *Recommended Development Environment* in `README.md` for the full setup). Sign in to GitHub in VS Code, then commit from the Source Control panel (Ctrl+Shift+G) → stage → write a message → Commit → Sync/Push. You can edit and commit this file the same way. **Pushing** matters: commits that are not pushed to GitHub are invisible to the instructor.

---

# Part A: Development Log (0.5 mark)

> ⚠️ **WARNING:** Minimum **5 entries**, spread over **different dates**. Five entries written on the same day, or written all at once at the end, will lose marks and look like a copy. Entry dates should be **between the start of the assignment and the deadline (November 14, 2026)**.
>
> 💡 **TIP:** Write an entry at the **end of each work session**, while you still remember what happened. It takes 5 minutes.
>
> 💡 **TIP:** Be specific. "Worked on the code" is a weak entry. "Added a `ReentrantLock queueLock` to `ReadyQueue` and wrapped the body of `poll()` in `lock()` / `try` / `finally { unlock() }`" is a strong one.
>
> 📌 **NOTE:** Each entry needs: date and time, what you did, details, challenges, solution, and time spent. Real challenges are fine (and expected). Do not invent fake ones.

## Example Entry (do not copy it, write your own)

### Entry 1 - [November 2, 2026, 4:30 PM]
**What I did**: Forked the repository, set my student ID, and ran the original starter

**Details**:
- Forked the starter repository and renamed it
- Changed student ID on line 304 to my actual ID (441234567)
- Ran the original program: 4 CPUs started, three of them picked `P1`, then `IllegalThreadStateException` and the watchdog stopped the program
- Saved the output in a text file for Question 1
- Committed and pushed: `Set my student ID: 441234567`

**Challenges**: I did not understand why the same process was picked by three CPUs

**Solution**: Read `ReadyQueue.poll()` again and found the `RaceWindow.pause()` between reading the head and removing it

**Time spent**: 45 minutes

---

## Your Development Log

> **Draft from the visible commit history:** The tasks and dates below are supported by the commits shown in the screenshots (November 9 and 11, 2026), but **exact session times, durations, and personal challenges must be confirmed by me before submission**. Commits made on the same date do not automatically prove separate work sessions. I should only keep entries that describe real sessions.

### Entry 1 - November 9, 2026, TODO: actual session time
**What I did**: Updated the student ID used for random number generation.

**Details**:
- Edited `SchedulerSimulationSync.java` to use my student ID as the simulation seed.
- My commit history includes `Update student ID for random number generation`.

**Challenges**: TODO — describe a challenge from this session, if any (do not invent one).

**Solution**: TODO — describe how I addressed that actual challenge; write "No major issue" if appropriate.

**Time spent**: TODO — approximate real duration.

---

### Entry 2 - November 9, 2026, TODO: actual session time
**What I did**: Worked on locks for the independent shared statistics.

**Details**:
- Added fine-grained locking around the shared counters.
- Used `contextLock`, `completedLock`, and `serviceLock` with `try/finally`.
- My commit history includes `Add fine-grained locks for shared variables`.

**Challenges**: TODO — fill in a real challenge from this session.

**Solution**: TODO — explain the actual fix or decision I made.

**Time spent**: TODO — approximate real duration.

---

### Entry 3 - November 11, 2026, TODO: actual session time
**What I did**: Protected the shared ready queue.

**Details**:
- Used a `ReentrantLock` named `queueLock` around the shared queue operations.
- Protected `add()`, `poll()`, `processOf()`, and `snapshot()` with `try/finally`.
- The commit history includes `Add lock for thread-safe access to ready queue`.

**Challenges**: TODO — fill in a real challenge from this session.

**Solution**: TODO — explain what I changed to address it.

**Time spent**: TODO — approximate real duration.

---

### Entry 4 - November 11, 2026, TODO: actual session time
**What I did**: Replaced repeated empty-queue polling with a counting semaphore.

**Details**:
- Added `readyCount = new Semaphore(0)` in `ReadyQueue`.
- Added `readyCount.release()` after `add()` and `readyCount.acquire()` inside `waitForProcess()`.
- Updated `CpuWorker.run()` to block on `waitForProcess()` instead of busy waiting.
- The commit history includes `Refactor run method to use blocking wait`.

**Challenges**: TODO — fill in a real challenge from this session.

**Solution**: TODO — explain the actual fix or decision I made.

**Time spent**: TODO — approximate real duration.

---

### Entry 5 - November 11, 2026, TODO: actual session time
**What I did**: Updated CPU shutdown and handling of unfinished processes.

**Details**:
- Added `wakeUpAllCPUs()` to release permits after the last process finishes.
- Kept unfinished processes moving back to the ready queue with `readyQueue.add(process)`.
- The commit history includes `Implement CPU wake-up on all processes completion` and `Add unfinished process back to ready queue`.

**Challenges**: TODO — fill in a real challenge from this session.

**Solution**: TODO — explain how I checked or resolved it.

**Time spent**: TODO — approximate real duration.

---

### Entry 6 - Optional — add a real additional work session if applicable
**What I did**: TODO — include only if this session really happened; otherwise remove this optional entry's content after confirming the lecturer allows it.

**Details**: TODO.

**Challenges**: TODO.

**Solution**: TODO.

**Time spent**: TODO.

---

## Development Log Summary

> 💡 **TIP:** Fill this in **last**, after all entries are written.

**Total time spent on assignment**: TODO — add up actual work sessions, not the time between commits.

**Most challenging part**: Suggested topic to personalize: making the blocked CPU threads exit cleanly when all processes are finished.

**Most interesting learning**: Suggested topic to personalize: the difference between protecting shared state with a lock and waiting for available work with a semaphore.

**What I would do differently next time**: TODO — add an honest observation from my own process.

---

# Part B: Reflection (0.5 mark)

> 🛑 **STOP:** Do **not** start this part until you have read the `README.md`, read the **entire** `SchedulerSimulationSync.java`, run it, and finished the three features.
>
> ⚠️ **WARNING:** Each answer must be **5 to 7 sentences**, in **your own words**. Copied or AI-generated answers without understanding get **0 marks for the whole assignment**. You may be asked to explain them in person.
>
> 💡 **TIP:** Mention concrete things you actually did: a method you wrote, an error you hit, a line of output you saw. Generic answers score low.
>
> 💡 **TIP:** Draft your answer in a few bullet points first, then turn them into sentences.

## Question 1: What did you learn about synchronization?

> 💡 **TIP:** Talk about race conditions (read-modify-write), critical sections, mutual exclusion with `ReentrantLock` and `try/finally`, the role of a counting semaphore, and what surprised you when the starter failed.

**Your Answer:** *(5-7 sentences)*

In this assignment, I learned that using multiple CPU threads can create race conditions when they share data. One example is `contextSwitchCount`, because reading a value and writing an increased value are separate steps. I used `ReentrantLock` to protect critical sections so that only one thread can change shared data at a time. I put `unlock()` in `finally` blocks because the lock should be released even if the protected code fails. I also learned that a counting semaphore is useful when workers need to wait for available processes instead of repeatedly checking the queue. The results helped me understand why synchronization is necessary, not just something added to make the code look safer.

## Question 2: What was the most challenging part of this assignment?

> 💡 **TIP:** Pick **one** specific challenge (understanding why the starter failed, choosing the lock granularity, the initial value of the semaphore, the shutdown of the CPUs, Git, the video) and say *why* it was hard.

**Your Answer:** *(5-7 sentences)*

The part I would choose as my main challenge was stopping CPU worker threads after the last process had finished. A semaphore can make a CPU wait correctly when there is no work, but that also means it might remain blocked at shutdown. I had to understand how `CpuWorker.run()` checks the completed-process counter after `waitForProcess()`. In my code, `wakeUpAllCPUs()` releases permits so blocked CPUs can wake up and check whether the simulation is finished. This was different from the ready-queue lock, because the problem was about waiting and termination rather than two CPUs changing a list together. I would explain this part using the `readyCount` semaphore and the final completed-process check in the code.

## Question 3: How did you overcome the challenges you faced?

> 💡 **TIP:** Describe your method: reading the slides and the documentation, adding `System.out.println` to debug, running the program many times, re-reading the README, testing after each small change, asking for help.

**Your Answer:** *(5-7 sentences)*

I focused on the methods that access shared data and checked where a lock or a semaphore was needed. For the queue, I examined `add()`, `poll()`, `processOf()`, and `snapshot()` instead of only locking one method. For the statistics, I used separate locks for the context-switch counter, completed-process counter, and total service time. I also reviewed how `waitForProcess()` blocks and how `wakeUpAllCPUs()` releases waiting CPU threads at shutdown. To check the result, the supplied modified Java file was compiled and run five times and the four verification values matched each time. Before submitting, I still need to confirm the same results from my GitHub version inside my IDE and describe any actual debugging steps I used.

## Question 4: Where can synchronization concepts be applied in real-world applications?

> 💡 **TIP:** Use real applications you know (banking and money transfers, ticket or seat booking, a shared counter on a website, a print queue, a database) and connect each one to what you built here (shared data, critical section, lock or semaphore).

**Your Answer:** *(5-7 sentences)*

Synchronization is useful anywhere multiple users or workers access the same data at the same time. In an online ticket-booking system, a lock can help stop two customers from claiming the same seat simultaneously. A banking system also needs to protect balance updates so that concurrent transfers do not overwrite each other. In a print server, a queue contains jobs that several workers may need to access safely. A semaphore can make workers sleep until new jobs are available, similar to `readyCount` in my scheduler. These examples connect to my project because both the ready queue and the shared statistics must remain consistent while multiple CPUs are running.

### Optional: What would you like to learn more about?

Optional — I can mention semaphore fairness, starvation, or deadlock if I genuinely want to explore them further.

### Optional: How confident do you feel about synchronization concepts now?

TODO (optional): choose my real confidence level and explain it in my own words.

### Optional: Feedback on the assignment

TODO (optional): add my own feedback, or mark this section N/A.

---

# Part C: Technical Answers (0.5 mark)

> 🛑 **STOP:** You cannot answer these questions without understanding the code. Re-read `SchedulerSimulationSync.java` and **run it** first. Your answers must reference **your own code and your own output** (your student ID makes your output and your expected values unique).
>
> ⚠️ **WARNING:** Each answer must be **3 to 5 sentences**, with specific examples from your code or output. Use correct terms: race condition, critical section, mutual exclusion, mutex lock, semaphore, busy waiting, deadlock, producer, consumer.
>
> 💡 **TIP:** Keep the output of the **original starter** and the output of your **final version** in text files or screenshots, so you can copy real snippets for Question 1.

## Question 1: Race Condition in Your Own Output

**Question**: Run the **original starter** (before any fix) and paste the **verification block** of that run. Which value was wrong (expected vs observed)? Explain **step by step**, with two named threads/CPUs, how **one lost update** happens on one of the shared variables (read, `RaceWindow.pause()`, write). Why can the same bug happen on a real machine even without `RaceWindow`, and why is it hard to detect?

> ⚠️ **WARNING:** The snippet must come from **your own run** (with your student ID), not from a classmate or from this README.
>
> 💡 **TIP:** Use a small timeline: *CPU-1 reads `contextSwitchCount` = 12 → CPU-2 reads 12 → CPU-1 writes 13 → CPU-2 writes 13 → one increment is lost.* If your starter run crashed before printing numbers, run it several times (or paste the exception and the watchdog message and explain it).

**Your Answer:** *(3-5 sentences)*

In the original starter, the shared updates and ready-queue operations were not protected, so the result could depend on which CPU ran first. In `incrementContextSwitch()`, two CPU threads could both read the same `contextSwitchCount` before either wrote its new value, causing a lost update. `RaceWindow.pause()` makes this timing problem easier to observe, but normal operating-system thread scheduling can cause the same overlap without that call. The exact failed line or exception from **my original starter run** must be included below before this explanation can describe my actual output accurately.

Verification block of the **original starter**:
```
TODO: Paste the ORIGINAL unmodified starter output using my student ID. If it crashed, paste the exception or watchdog message instead. Do not substitute the example from the instructions.
```

Verification block of **my final version** (five local test runs of the supplied code; reproduce in my IDE before submitting):
```
Context switches (quanta executed)   expected 38       observed 38       ✔
Completed processes                  expected 19       observed 19       ✔
Total service time (ms)              expected 112348   observed 112348   ✔
Busy-waiting polls (must be 0)       expected 0        observed 0        ✔
✔ All shared values are consistent.
```

**Explanation of the timeline:**
Illustrative interleaving (not a quotation from my output): CPU-1 reads `contextSwitchCount = 12`, then `RaceWindow.pause()` allows CPU-2 to read the same 12; CPU-1 writes 13 and CPU-2 also writes 13. The correct total after two increments is 14, but the stored total is only 13, so one update is lost.

## Question 2: Critical Sections and Lock Granularity

**Question**: List the **critical sections** you protected (variables and methods) and the lock(s) you used. **Lock granularity:** did you use **one lock** for the three statistics or **one lock per variable**? Why, and what is the trade-off? Why is the **ready queue** protected by a **different** lock than the statistics? Explain how your solution provides **mutual exclusion**, and discuss **progress** and **bounded waiting** (a default `ReentrantLock` is not fair: what does that imply?).

> 💡 **TIP:** The three counters are independent: does updating `contextSwitchCount` need to block an update of `totalServiceTime`? Also think about what could go wrong (deadlock, or long waiting) if the queue lock and the statistics lock were the **same** lock and a thread held it while doing something slow.

**Your Answer:** *(3-5 sentences)*

I protected `ReadyQueue.add()`, `poll()`, `processOf()`, and `snapshot()` with `queueLock` because they access the shared list or map. For statistics, I used a different `ReentrantLock` for each variable and protected both its update and its getter, which allows unrelated counters to be updated in parallel but requires more lock objects. Keeping `queueLock` separate prevents queue operations from being delayed by statistics updates, while `lock()` and `unlock()` in `try/finally` provide mutual exclusion for each critical section. Short critical sections help threads make progress when the lock is released, but this does not guarantee every waiting thread will be served in a strict order. Because the default `ReentrantLock` is non-fair, bounded waiting is not guaranteed and a thread might wait longer than other threads under contention.

| Critical section (variable / method) | Lock used | Why it needs protection |
|---|---|---|
| `ReadyQueue.add()` and `poll()` | `queueLock` | Adding and removing queue items must not race |
| `ReadyQueue.processOf()` and `snapshot()` | `queueLock` | Reading shared queue/map contents must be consistent |
| `SharedStats.incrementContextSwitch()` and `getContextSwitchCount()` | `contextLock` | Protect the context-switch count from lost updates and unsynchronized reads |
| `SharedStats.incrementCompletedProcess()` and `getCompletedProcessCount()` | `completedLock` | Protect the completed-process count and shutdown checks |
| `SharedStats.addServiceTime()` and `getTotalServiceTime()` | `serviceLock` | Protect the accumulated service time from lost updates |

## Question 3: Busy Waiting vs Semaphore

**Question**: Describe the **busy waiting** of the starter and its cost (give the `Busy-waiting polls` number from your **starter** run). What does the **value of your semaphore** represent? What is its **initial value** and why? What is its value right after the `numProcesses` initial `add()` calls? Why does the last CPU call `release(totalCPUs)` at the end, and what would happen if it did not?

> 💡 **TIP:** Think about what a CPU does when the queue is empty in the starter, and what a CPU does in your final version (is it running, ready or blocked?). Also check what happens to a CPU blocked in `acquire()` when no process will ever be added again.

**Your Answer:** *(3-5 sentences)*

The original worker loop repeatedly checked the ready queue when it was empty, causing busy waiting and using CPU time; the `Busy-waiting polls` value in my original run was **TODO: enter the real number**. In my version, `readyCount` starts at 0 because no processes have been added yet, and each call to `add()` releases one permit to represent a queued process. After the 19 initial `add()` calls and before the CPUs start, the semaphore has 19 permits; when a CPU calls `acquire()`, it takes a permit or blocks until one is available. When the final process completes, `wakeUpAllCPUs()` calls `release(SharedStats.totalCPUs)` so blocked workers can wake and exit after checking the completed-process count. Without that shutdown release, a waiting worker could stay blocked forever and trigger the watchdog.

## Question 4: Classical Problems and Deadlock

**Question**: The CPUs and the ready queue look like a classical synchronization problem of Chapter 5. **Name it**, and say who plays the **producer** and the **consumer** roles (careful: here the CPUs also re-enqueue processes). If the ready queue were **bounded** (capacity `K`), name the **three semaphores** you would need and their **initial values**. Describe a **deadlock scenario** that appears if a thread acquired the **mutex before** waiting on the semaphore (or if two locks were acquired in different orders), and say **which of the four necessary conditions** you would break to prevent it.

> 💡 **TIP:** Recall the bounded-buffer solution of the slides (`empty`, `full`, `mutex`) and the order of `wait()` calls in the producer and the consumer. For the deadlock, think about a producer that holds the mutex while waiting for a free slot that only a consumer (who needs the mutex) can create.

**Your Answer:** *(3-5 sentences)*

This is the producer-consumer problem: the main thread adds the initial processes as a producer, while CPUs consume items from the ready queue and also become producers when they re-enqueue unfinished processes. If the queue had a maximum capacity `K`, it would need three semaphores: `empty = K`, `full = 0`, and `mutex = 1`. A producer that acquires `mutex` before waiting on `empty` could hold the mutex when the buffer is full, stopping the consumer from taking an item and making space. Acquiring the counting semaphore before the mutex prevents that hold-and-wait deadlock, and a consistent acquisition order can also prevent circular wait when using multiple locks.

**Classical problem and roles**:
Producer-consumer: main produces the initial queue items; CPUs consume queued processes and produce new queue items when unfinished processes are re-enqueued.

**Semaphores for a bounded queue (name and initial value)**:
`empty = K`, `full = 0`, `mutex = 1` (hypothetical bounded queue).

**Deadlock scenario and prevention**:
If a producer holds `mutex` while waiting for a free slot, the consumer cannot enter the critical section to create a slot. Acquire `empty` before `mutex` to avoid holding the mutex while waiting, breaking the hold-and-wait condition for this scenario; use consistent lock order to avoid circular wait with multiple locks.

## Summary

**Key concepts I understood through these questions:**
1. Race conditions and mutual exclusion for shared state
2. Fine-grained locks and safe critical sections with `try/finally`
3. Counting semaphores, CPU blocking, and clean shutdown

**Concepts I need to study more:**
1. Fairness and starvation with non-fair locks (edit if needed)
2. Deadlock prevention in bounded-buffer systems (edit if needed)

---

# ✅ Final Checklist (complete before submitting)

> ⚠️ **WARNING:** Go through every line. Blackboard does not accept submissions after the deadline, which is **November 14, 2026**.

**Repository**
- [ ] Repository is **PUBLIC** (Settings → Danger Zone → Visibility)
- [ ] Repository is renamed to `OS-Assignment3-YourFirstName-YourLastName`
- [ ] GitHub account uses the university email (`@std.psau.edu.sa`)

**Code**
- [ ] Student ID is set in `SchedulerSimulationSync.java` (line 304)
- [ ] My code is based **only** on the starter of this repository (nothing copied from previous assignments)
- [ ] Code compiles and runs with no errors, and terminates by itself (no `⛔ WATCHDOG`)
- [ ] Feature 1 (ready queue lock), Feature 2 (statistics locks) and Feature 3 (semaphore, no busy waiting) all work
- [ ] **The four verification lines are ✔ in 5 consecutive runs**
- [ ] Every lock is released in a `finally` block
- [ ] `RaceWindow`, `Config`, the verification block and the watchdog are **unchanged**
- [ ] Each feature has clear comments

**Commits**
- [ ] **At least 4 meaningful commits, ideally 7 or more**
- [ ] **One commit per feature**
- [ ] Commits are spread over **different dates** (not all in the last hour)
- [ ] Everything is **pushed** to GitHub

**This file (`MY_WORK.md`)**
- [ ] Full name and student ID filled in at the top
- [ ] Development log has **5+ entries** on different dates
- [ ] Reflection: 4 questions, 5-7 sentences each
- [ ] Technical answers: 4 questions, 3-5 sentences each, with examples from **your** output (starter output **and** final output pasted in Question 1)
- [ ] No `[...]` placeholders left
- [ ] No section headers deleted

**Video**
- [ ] 2-3 minutes long, named `StudentID_Assignment3_Demo.mp4`
- [ ] Shows your name, ID, repository, 3 features (and your lock granularity choice), IDE execution with the verification block, one synchronization concept, and commit history
- [ ] Link is **public** (tested in an incognito window) and pasted in the **Video Link** section above

**Blackboard**
- [ ] Submit **only** the link to your public GitHub repository

> 🎯 **Good luck!** Start early, commit regularly, and make sure you can explain every line you submit.
