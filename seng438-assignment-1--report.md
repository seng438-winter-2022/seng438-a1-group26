> **SENG 438 - Software Testing, Reliability, and Quality**

**Lab. Report \#1 – Introduction to Testing and Defect Tracking**

| Group 26         |          |                |
| ---------------- | -------- | -------------- |
| Liana Goodman    | 30089196 | LianaBG        |
| Amir Abdrakmanov | 30085827 | aabdrakmanov   |
| Jared Lundy      | 30086687 | jared840       |
| Jordan Lundy     | 30086686 | jordan427-prog |

**Table of Contents**

[1 Introduction](#introduction)

[2 High-level description of the exploratory testing plan](#high-level-description-of-the-exploratory-testing-plan)

[3 Comparison of exploratory and manual functional testing](#comparison-of-exploratory-and-manual-functional-testing)

[4 Notes and discussion of the peer reviews of defect reports](#notes-and-discussion-of-the-peer-reviews-of-defect-reports)

[5 How the pair testing was managed and team work/effort was
divided](#how-the-pair-testing-was-managed-and-team-workeffor-was-divided)

[6 Difficulties encountered, challenges overcome, and lessons
learned](#difficulties-encountered-challenges-overcome-and-lessons-learned)

[7 Comments/feedback on the lab and lab document itself](#commentsfeedback-on-the-lab-and-lab-document-itself)

# Introduction

Before beginning these lab axercises and the associated documentation, our group new a few things about manual script and exploratory testing.

Primarily, we knew that exploratory testing allows users to explore the system creatively and to find their own issues based on how they might use the system, while manual scripted testing allows for comparison of results to both a known expected result and to results from previous (or subsequent) versions.

Exploratory testing is most useful when done by people who were not on the development team and are unfamiliar with the system. It provides an insight into functionalities that users may try to work with and shows how the system may be used without instructions. This creative approach is sure to find bugs that developers may have missed due to familiarity with the system. It might also help reveal design flaws or UI flaws that, though not technically wrong, can greatly affect the user's ability to use, understand, and enjoy the program.

Manual testing allows testers to use the system as intended, using knowledge about how the system should be behaving. This kind of testing displays bugs that interfere with the intended development but may miss additional bugs that interfere with the whole system. Testing with knowledge of the system allows testers to easily identify bugs as flaws instead of as a simple misunderstanding of the intended purpose of the system. Testers who know exactly what the expected output is, will be able to provide very clear details on what the issues are. Additionally, these tests will be the easiest to replicate as exploratory testing may be difficult to replicate if insufficient instructions are provided.

A combination of these two test styles will allow for a thorough discovery of bugs, as long as all testers are careful in tracking their work and are test all of their ideas. Since the testing styles are so different, they are very complimentary.

# High-level description of the exploratory testing plan

Motivation:
The initial exploratory testing phase is meant to both explore the system under test, while also identifying a large amount of bugs in the system.
Since the exploratory phase does not have any script, the goal is therefore to find as many initial bugs as possible in a flexible manner.
The flexibility of this step should allow us to be creative in finding the bugs within the system and also becoming very comfortable with the workings
of the system along the way.

Functions being targeted: 
- Customer cash withdrawal 
- Customer cash deposit, both with cash and with checks 
- Customer money transfer between two accounts 
- Customer balance inquiry 
- Customer aborting transaction in progress 
- Invalid pin response

Testing Approach:
The exploratory testing approach will be to test every function a little bit to find evident bugs throughout the
system's operation. This will allow us to gather an extensive list of the most general bugs, and gives us the best
exploration/overview of the system's defects. Thus, the most crucial errors in the system should be revealed in this testing,
and ensures the biggest defects are found.

Test Case paths:
The test cases will be created using the most common paths for the system. This should, as previously stated, allow this exploratory testing
to best cover the most general and important bugs in the system, while simultaneously allowing us to best explore the system.

# Comparison of exploratory and manual functional testing

When compared to manual scripted testing, exploratory testing has both benefits and drawbacks. One benefit of exploratory testing is the relative flexibility provided to those performing it. Due to exploratory testing having little formal structure, it gives the programmers creativity to find as many bugs as possible and also gives them a great opportunity to explore the system under test. For an experienced programmer, this is a benefit, as they have the liberty to immediately search for bugs that they feel other programmers may have missed. Thus, it gives software engineers to ability to use their coding expertise to find bugs. Our group found that this allowed us to find many bugs in the exploratory testing phase, since it allowed us to do whatever was needed to explore and subsequently identify defects within the system. 

However, the flexible nature of exploratory testing also became a slight drawback later on in the testing phase, where it became increasingly harder to discover more bugs. Manual functional testing provided a uniform sense of consistency throughout its testing phase since each test case was well defined from the first to the last manual test case via the test suite. It also provided a clear understanding of the main functions of the program which provided clear repeat testing for subsequent versions.

In terms of effectiveness, both testing methods proved effective in finding defects. However, based on our backlog bug tracking, exploratory testing seemed to unearth more bugs than manual testing. Efficiency-wise, manual testing edged out exploratory due to the test suite. Since the suite told us exactly what tests to do, there was no time wasted trying to think of new tests or possible bugs.

A record of our bugs can be found in the main folder in `Defect-Report.xlsx` which is in the main folder.

# Notes and discussion of the peer reviews of defect reports

Defect reports were create on backlog, on the space: https://seng438-x.backlog.com/ with email amir.abdrakmanov@ucalgary.ca, username Lab1-GroupX and password Seng438Assignments. Here X was a place holder since this was created before the group number (group 26) was given.

After teams completed the first round of testing on version 1.0, both teams would review each other's defects reports and test them on version 1.1. Some reports found were duplicate with another report, those were deleted. Others were somewhat simliar, these simliar reports were merged when possible, otherwise left alone. Some reports however were found to not be of the highest quality, those were also deleted or edited to contain greater detail.

As the system under test updated to 1.1, new bugs were found and added to the report. These defects are marked as "open" in backlog.

The way the defect reports were reveiwed was pair based so that each team could see and review the defects with a "fresh set of eyes"

# How the pair testing was managed and team work/effort was divided

Team work was divided as evenly as possible, with both pairs doing one round of exploratory testing and both pairs doing one round of manual scripted testing. The manual scripted testing was split up so that one group would run the tests on version 1.0 and one group would run the tests on version 1.1. Additionally, the groups did reverse testing order with one group starting with exploratory and the other group starting with scripted testing. This made sure that the groups approached testing differently and increased the number of bugs we may find.

After the groups had completed individual testing of version 1.0, we all got together and compared our bugs found. Then we all added the bugs to BackLog to ensure our bugs were properly tracked.

Following our logging of bugs, we broke back into pairs to do a second round of exploratory testing with greater knowledge of the system and some ideas of features which may need to be explored more.

Afterwards, the scripted testing of version 1.1 was completed. From there, the pairs got back together to discuss the results and compile the report.

# Difficulties encountered, challenges overcome, and lessons learned

One of the difficulties encountered in this lab was determining, especially in exploratory, if a bug was new or a repeated bug showing up in another test case.
Another difficulty in this lab was thinking of new test cases once many had already been explored.

Another difficuly faced was keeping track of the actual values that should be in the accounts throughout the tests, as testing deposits and withdrawals/deposits frequently changed what was in the accounts and checking the altered values required us to remember the previous correct value.

We also found it difficult at times to determine whether or not an action of the simulation was a bug or a how it was supposed to run. When in doubt here, we asked ourselves what a real machine would do and whether or not it was feasible for this to happen.

# Comments/feedback on the lab and lab document itself

Overall, this lab was useful because not only did it explain in detail exploratory, manual scripted and regression testing, but it allowed us to actually perform iterations of these tests firsthand, as well as gain valuable
experience with a bug tracking tool. Getting this firsthand experience with these tests gave us a much more detailed understanding of these testing methods, and allows us the opportunity to now apply these testing methods towards other software, whether it being our own or someone else's.

The lab instructions were relatively easy to follow as well.
