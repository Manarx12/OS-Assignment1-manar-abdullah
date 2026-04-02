# Development Log

## Instructions
Document your development process as you work on the assignment. Add entries showing:
- What you worked on
- Problems you encountered
- How you solved them
- Time spent

**Requirements**: Minimum 5 entries showing progression over time.

---

## Example Entry Format:

### Entry 1 - [April 1, 2026, 2:30 PM]
**What I did**: Forked the repository and set up my student ID

**Details**: 
- Created GitHub account with university email
- Forked the starter repository
- Changed student ID on line 92 to my actual ID (441234567)
- Compiled and ran the program successfully

**Challenges**: Had to install JDK first because javac wasn't recognized

**Solution**: Downloaded JDK 17 from Oracle website and set PATH variable

**Time spent**: 30 minutes

---

## Your Development Log:

Entry 1 - [2026-04-01 - 4:00 PM]
What I did: Project Setup and Forking.

Details: I forked the assignment repository from GitHub to my personal account and cloned it locally using VS Code.

Challenges: I initially had trouble finding the fork button and faced an error when trying to clone the file name instead of the URL.

Solution: I used the correct HTTPS URL from the green "Code" button on GitHub and successfully cloned the repository.

Time spent: 1 hour.

Entry 2 - [2026-04-01 - 6:00 PM]
What I did: Student ID Customization.

Details: I updated the studentID variable in SchedulerSimulation.java to my actual ID: 445052716.

Challenges: Locating the exact line in the code.

Solution: I used the search function (Ctrl+F) to find the studentID variable and changed it to seed the random generator.

Time spent: 30 minutes.

Entry 3 - [2026-04-02 - 10:00 AM]
What I did: Implementing Feature 1 (Priority).

Details: I added a priority field to the Process class and updated the constructor to assign a random priority (1-5) to each process.

Challenges: Making sure the priority was displayed correctly in the terminal output.

Solution: I updated the addProcessToQueue method in SchedulerSimulation.java to print the priority alongside the process name.

Time spent: 1.5 hours.

Entry 4 - [2026-04-02 - 2:00 PM]
What I did: Implementing Feature 2 (Context Switch Counter).

Details: I created a static variable contextSwitches and incremented it every time a process was pulled from the queue.

Challenges: Placing the counter in the correct location within the while loop.

Solution: I placed the increment logic right after the processQueue.poll() call to count every time the CPU switches tasks.

Time spent: 1 hour.

Entry 5 - [2026-04-02 - 8:00 PM]
What I did: Implementing Feature 3 (Waiting Time Table).

Details: I added a startTime variable to the Process class and created a formatted summary table at the end of the simulation.

Challenges: Encountering "cannot be resolved" errors for PURPLE and allProcessesList.

Solution: I used MAGENTA instead of PURPLE and used the existing processMap to iterate through all processes and calculate their waiting times.

Time spent: 2 hours.

Entry 6 - [2026-04-02 - 10:30 PM]
What I did: Final Documentation and Push.

Details: I filled out the ANSWERS.md file with theoretical answers and pushed all changes back to my GitHub repository.

Challenges: Using Git commands for the first time.

Solution: I used git add, git commit, and git push in the VS Code terminal to sync my work.

Time spent: 1 hour.

Summary
Total time spent on assignment: 7 hours.

Most challenging part: Handling Java errors when adding Feature 3 and calculating the exact waiting time for each process correctly.

Most interesting learning: Learning how the Round Robin algorithm actually manages multiple threads and how context switching impacts system performance.

What I would do differently: I would spend more time reading the Java Extension Pack documentation earlier to avoid the initial setup confusion in VS Code.erently next time**: 
