# FullStack-Collaborative-THRON-S-5

# Programming Quiz Platform

A full-stack Django-based Programming Quiz Platform designed for students to practice, evaluate, and improve their programming knowledge through structured quizzes.

The project is based on an existing Online Quiz System. Students will collaboratively extend and redesign the existing application into a complete Programming Quiz Platform while preserving stable existing functionality.

---

# 1. Project Objective

The objective of this project is to transform the existing Online Quiz System into a modern Programming Quiz Platform.

The platform should allow:

- Students to register and log in
- Students to select programming languages
- Students to select quiz difficulty
- Students to take programming quizzes
- Questions to be presented in a controlled/randomized manner
- Students to receive scores after completing quizzes
- Students to review their answers
- Students to view previous attempts
- Students to track their progress
- Teachers to create and manage programming quizzes
- Teachers to create and manage programming questions
- Administrators to manage the complete platform
- Administrators and teachers to view quiz performance
- Students to compare performance through a leaderboard

The final system should have a professional, responsive and attractive user interface.

---

# 2. Existing Project

The existing project is a Django Online Quiz System.

The existing application contains functionality related to:

- Student registration
- Student login
- Teacher registration/login
- Admin management
- Courses
- Exams
- Questions
- Results
- Student dashboard
- Teacher dashboard
- Admin dashboard

The existing project should be treated as the starting point.

## Important

Do not unnecessarily delete or rewrite existing working functionality.

Before modifying any module:

1. Understand the existing code.
2. Identify dependencies.
3. Check related URLs.
4. Check related views.
5. Check related templates.
6. Check related models.
7. Modify only what is required.
8. Test the application after the modification.

---

# 3. Target Platform

The final application will be called:

## Programming Quiz Platform

The platform should focus primarily on programming-related quizzes.

---

# 4. Main User Roles

The application will have three primary roles:

```text
Student
Teacher
Admin
````

---

# 5. Overall System Workflow

```text
                         PROGRAMMING QUIZ PLATFORM
                                    |
                 +------------------+------------------+
                 |                  |                  |
                HOME             STUDENT            TEACHER
                 |                  |                  |
                 |              Register/Login    Register/Login
                 |                  |                  |
                 |             Student Dashboard   Admin Approval
                 |                  |                  |
                 |            Select Language     Teacher Dashboard
                 |                  |                  |
                 |            Select Difficulty        |
                 |                  |                  |
                 |            Select Quiz              |
                 |                  |                  |
                 |            Quiz Instructions        |
                 |                  |                  |
                 |              Start Quiz             |
                 |                  |                  |
                 |            Answer Questions         |
                 |                  |                  |
                 |            Submit Quiz              |
                 |                  |                  |
                 |            Calculate Score           |
                 |                  |                  |
                 |              Result                  |
                 |                  |                  |
                 |       Review / Attempt History       |
                 |                  |                  |
                 |             Leaderboard               |
                 |                                          
                 |
                ADMIN
                 |
             Admin Login
                 |
          Admin Dashboard
                 |
      +----------+----------+
      |          |          |
    Users    Languages    Quizzes
                 |
             Questions
                 |
             Analytics
```

---

# 6. Home Page

The homepage should act as the main entry point of the platform.

## Required Sections

### Navigation Bar

Navigation should contain appropriate links such as:

* Home
* Programming
* Quizzes
* Leaderboard
* About
* Contact
* Login
* Get Started

The exact navigation can be adjusted based on the final implementation.

---

## Hero Section

The hero section should contain:

* Main platform title
* Short description
* Start Quiz button
* Explore Quizzes button
* Programming-related visual/image

Example concept:

```text
Test Your Code

Challenge yourself with programming quizzes,
improve your technical knowledge and build
confidence through practice.

[ Start Quiz ] [ Explore Quizzes ]
```

---

# 7. Programming Languages

The platform should support programming categories.

Initial categories:

```text
C
C++
Java
Python
JavaScript
HTML
CSS
SQL
```

The system should be designed so additional languages can be added later.

Each language may contain:

* Name
* Description
* Image
* Icon/visual
* Status
* Display order

---

# 8. Difficulty Levels

Each quiz should support difficulty levels.

Required levels:

```text
Beginner
Intermediate
Advanced
```

A student should be able to filter/select quizzes based on difficulty.

---

# 9. Student Registration

Students should be able to create an account.

Required information may include:

```text
Name
Email
Password
Phone
Profile Image
```

The implementation should preserve the existing registration system where possible.

---

# 10. Student Login

Students should be able to:

```text
Login
Logout
Access Dashboard
View Profile
```

Authentication should continue using Django's existing authentication architecture where possible.

---

# 11. Student Dashboard

After login, students should see a dashboard containing:

```text
Welcome Section

Statistics
    |
    +-- Quizzes Attempted
    +-- Quizzes Completed
    +-- Average Score
    +-- Best Score
    +-- Overall Progress

Continue Learning

Recommended Quizzes

Recent Attempts

Programming Languages

Leaderboard
```

---

# 12. Language Selection Workflow

The student should be able to select a programming language.

Example:

```text
Programming
     |
     +-- C
     +-- C++
     +-- Java
     +-- Python
     +-- JavaScript
     +-- HTML
     +-- CSS
     +-- SQL
```

After selecting a language:

```text
Python
   |
   +-- Beginner
   +-- Intermediate
   +-- Advanced
```

---

# 13. Quiz Listing

After selecting a language and difficulty, the student should see available quizzes.

Example:

```text
Python

Beginner
    |
    +-- Python Basics
    +-- Python Variables
    +-- Python Operators

Intermediate
    |
    +-- Python Functions
    +-- Python OOP
    +-- Python Data Structures

Advanced
    |
    +-- Advanced Python
    +-- Python Problem Solving
```

Each quiz card should display relevant information such as:

* Quiz name
* Language
* Difficulty
* Number of questions
* Duration
* Passing percentage
* Description

---

# 14. Quiz Details Page

Before starting a quiz, display:

```text
Quiz Name

Language:
Python

Difficulty:
Intermediate

Questions:
20

Duration:
20 Minutes

Total Marks:
20

Passing Score:
50%

Description
```

Button:

```text
Start Quiz
```

---

# 15. Quiz Engine

The quiz engine is one of the most important modules.

The quiz should support:

* Multiple-choice questions
* Question navigation
* Timer
* Progress indicator
* Answer selection
* Previous question
* Next question
* Submit quiz
* Automatic score calculation

Example:

```text
Python Functions

Question 4 / 20

Time Remaining: 15:42

What will be the output?

def test():
    return 10

print(test())

A. 10
B. None
C. Error
D. test

[Previous] [Next]
```

---

# 16. Random Question Selection

Questions should be capable of being randomized.

Example:

```text
Question Bank
      |
Filter by:
      |
Language
      |
Difficulty
      |
Quiz
      |
Random Selection
      |
Selected Questions
      |
Student
```

Different attempts may contain different question orders or question selections.

Example:

```text
Attempt 1:
Q3 Q27 Q41 Q56 Q72

Attempt 2:
Q8 Q19 Q33 Q48 Q91
```

The exact randomization strategy should be finalized during implementation.

---

# 17. Question Types

The initial implementation should support:

## Type 1 — Multiple Choice

```text
Question

A. Option A
B. Option B
C. Option C
D. Option D

Correct Answer: B
```

---

## Type 2 — True / False

Example:

```text
Python is dynamically typed.

A. True
B. False
```

---

## Type 3 — Code Output

Example:

```text
What will be the output?

def add(a, b):
    return a + b

print(add(2, 3))

A. 4
B. 5
C. 6
D. Error
```

---

## Future Question Types

These may be implemented later:

* Multiple correct answers
* Debugging questions
* Fill-in-the-code
* Code completion
* Programming problems

Do not implement these unless they are assigned as part of the project phase.

---

# 18. Question Structure

A programming question should support fields such as:

```text
Question
Language
Topic
Difficulty
Question Type

Option A
Option B
Option C
Option D

Correct Answer
Marks

Explanation
```

Example:

```text
Language:
Python

Topic:
Functions

Difficulty:
Intermediate

Question:
What will this code output?

Code:
def add(a, b):
    return a + b

print(add(2, 3))

Option A:
4

Option B:
5

Option C:
6

Option D:
7

Correct Answer:
B

Marks:
1

Explanation:
The function returns the sum of the two arguments.
```

---

# 19. Timer

Each quiz may have a configured time limit.

Example:

```text
Quiz Duration: 20 Minutes

20:00
19:59
19:58
...
00:10
00:09
...
00:00
```

When the timer reaches zero:

```text
Automatically Submit Quiz
```

The timer should not be implemented in a way that can easily be bypassed through simple browser manipulation.

---

# 20. Quiz Submission

When the student selects Submit:

```text
Submit Quiz
     |
Confirmation
     |
Calculate Score
     |
Save Attempt
     |
Save Answers
     |
Generate Result
```

The attempt should be stored in the database.

---

# 21. Result Page

After submission:

```text
Python Functions

Score:
17 / 20

Percentage:
85%

Status:
Passed

Correct:
17

Incorrect:
3

Unanswered:
0

Time Taken:
14:21
```

Buttons:

```text
Review Answers
Try Again
Back to Dashboard
```

---

# 22. Answer Review

Students should be able to review their submitted answers.

Example:

```text
Question 1

Question:
What does len() return?

Your Answer:
Number of elements

Correct Answer:
Number of elements

Status:
Correct
```

For an incorrect answer:

```text
Your Answer:
Option B

Correct Answer:
Option C

Explanation:
...
```

The explanation field should be displayed when available.

---

# 23. Attempt History

Students should be able to see previous attempts.

Example:

```text
My Attempts

Quiz                 Score      Date       Status
--------------------------------------------------
Python Functions     85%        Sep 27     Passed
C Pointers           70%        Sep 25     Passed
Java OOP             40%        Sep 22     Failed
```

Each attempt should provide an option to view the result.

---

# 24. Student Progress

The student dashboard should eventually show:

```text
Overall Progress

Average Score
Best Score
Total Attempts
Passed Quizzes
Failed Quizzes

Language Performance

Python      85%
Java        72%
C           68%
C++         81%
```

---

# 25. Leaderboard

The platform may include a leaderboard.

Example:

```text
Leaderboard

Rank    Student       Score
---------------------------
1       Student A     95%
2       Student B     92%
3       Student C     89%
4       Student D     87%
```

Possible filters:

```text
Overall
Python
Java
C++
Weekly
Monthly
```

Leaderboard rules should be clearly defined before implementation.

---

# 26. Teacher Workflow

Teacher workflow:

```text
Teacher Registration
        |
Admin Approval
        |
Teacher Login
        |
Teacher Dashboard
```

---

# 27. Teacher Dashboard

The teacher dashboard should provide:

```text
Total Quizzes
Total Questions
Total Students
Total Attempts
Average Score
```

Teacher management options:

```text
Create Quiz
Manage Quizzes
Add Questions
Manage Questions
View Results
View Student Performance
```

---

# 28. Teacher — Create Quiz

Teacher should be able to create:

```text
Quiz Name
Description
Language
Difficulty
Number of Questions
Time Limit
Passing Percentage
Status
```

Example:

```text
Quiz Name:
Python Functions

Language:
Python

Difficulty:
Intermediate

Questions:
20

Duration:
20 Minutes

Passing:
50%
```

---

# 29. Teacher — Add Questions

Teacher should be able to add programming questions.

Required fields:

```text
Language
Topic
Difficulty
Question Type
Question
Code
Option A
Option B
Option C
Option D
Correct Answer
Marks
Explanation
```

The `Code` field should be optional for normal MCQ questions.

---

# 30. Teacher — Quiz Management

Teacher should be able to:

```text
Create Quiz
Edit Quiz
Delete Quiz
Publish Quiz
Unpublish Quiz
View Questions
Add Questions
Edit Questions
Delete Questions
View Attempts
```

---

# 31. Teacher Analytics

Teachers should eventually be able to view:

```text
Average Score
Highest Score
Lowest Score
Pass Rate
Total Attempts
Question Accuracy
```

Example:

```text
Python Functions

Average Score: 74%

Highest Score: 98%

Lowest Score: 31%

Pass Rate: 72%

Total Attempts: 184
```

---

# 32. Admin Workflow

Admin:

```text
Admin Login
      |
Admin Dashboard
```

Admin should have complete platform control.

---

# 33. Admin Management

Admin modules:

```text
Students
Teachers
Programming Languages
Quizzes
Questions
Attempts
Results
Analytics
```

---

# 34. Admin — Student Management

Admin should be able to:

```text
View Students
Search Students
View Student Profile
Activate Student
Deactivate Student
Delete Student
View Student Attempts
```

---

# 35. Admin — Teacher Management

Admin should be able to:

```text
View Teachers
Approve Teachers
Reject Teachers
Activate Teacher
Deactivate Teacher
Delete Teacher
```

---

# 36. Admin — Programming Language Management

Admin should be able to:

```text
Add Language
Edit Language
Delete Language
Enable Language
Disable Language
Change Display Order
```

Possible fields:

```text
Language Name
Slug
Description
Image
Status
Display Order
```

---

# 37. Admin — Quiz Management

Admin should be able to:

```text
Create Quiz
Edit Quiz
Delete Quiz
Publish Quiz
Unpublish Quiz
View Questions
View Attempts
```

---

# 38. Admin — Question Management

Admin should be able to:

```text
Add Question
Edit Question
Delete Question
Change Difficulty
Change Language
Change Question Type
Set Correct Answer
Set Marks
Add Explanation
```

---

# 39. Admin Analytics

Admin dashboard should eventually display:

```text
Total Students
Total Teachers
Total Languages
Total Quizzes
Total Questions
Total Attempts

Average Score
Pass Rate
Most Popular Language
Most Attempted Quiz
Most Difficult Quiz
```

---

# 40. Image System

Images will be supplied separately.

Images may be used for:

```text
Homepage
Programming Languages
Quiz Cards
Dashboard
Banners
Sections
```

Recommended static structure:

```text
static/
│
└── images/
    │
    ├── home/
    │
    ├── languages/
    │   ├── python/
    │   ├── java/
    │   ├── c/
    │   ├── cpp/
    │   └── javascript/
    │
    ├── quizzes/
    │
    ├── dashboard/
    │
    └── banners/
```

Do not download random images without approval.

Use the images provided for the project.

---

# 41. UI/UX Requirements

The final website should have a professional modern interface.

Required:

* Responsive design
* Desktop support
* Tablet support
* Mobile support
* Clean navigation
* Consistent typography
* Consistent spacing
* Attractive quiz cards
* Interactive buttons
* Hover effects
* Smooth transitions
* Progress indicators
* Professional dashboards
* Proper form validation

Animations should improve the interface without making it difficult to use.

---

# 42. No Emoji Requirement

Do not use emojis anywhere in the website unless specifically requested.

Attraction should be created using:

* CSS animations
* Transitions
* Images
* Typography
* Layout
* Cards
* Gradients
* Shadows
* Interactive elements
* Icons only when specifically approved

---

# 43. Suggested Database Architecture

The existing application should be analyzed before modifying the database.

Target conceptual structure:

```text
User
 |
 +---- Student
 |
 +---- Teacher
 |
 +---- Admin
```

```text
ProgrammingLanguage
        |
        +---- Quiz
                |
                +---- Question
```

```text
Student
   |
   +---- QuizAttempt
            |
            +---- AttemptAnswer
                    |
                    +---- Question
```

Possible entities:

```text
User
Student
Teacher

ProgrammingLanguage

Quiz
Question

QuizAttempt
AttemptAnswer

Result
```

Do not create duplicate models if an existing model can safely be extended.

---

# 44. Development Rule — Protect Existing Functionality

This is a collaborative student project.

Before changing any file:

```text
Read
  ↓
Understand
  ↓
Identify dependencies
  ↓
Modify
  ↓
Run
  ↓
Test
```

Do not blindly replace files.

Do not delete working functionality without approval.

Do not modify database models without checking related migrations.

Do not modify URLs without checking corresponding views and templates.

Do not change authentication without checking all user roles.

---

# 45. Git Collaboration Rules

Each team member should work on a separate branch.

Example:

```text
main
│
├── feature/homepage
├── feature/student-dashboard
├── feature/quiz-engine
├── feature/question-management
├── feature/teacher-dashboard
├── feature/admin-dashboard
└── feature/leaderboard
```

Do not directly push experimental changes to `main`.

---

# 46. Suggested Team Responsibilities

## Team Member 1 — UI / Homepage

Responsible for:

```text
Homepage
Navbar
Footer
Programming Categories
Landing Page
Animations
Responsive Design
```

---

## Team Member 2 — Student Module

Responsible for:

```text
Student Registration
Student Login
Student Dashboard
Profile
Progress
Attempt History
```

---

## Team Member 3 — Quiz Engine

Responsible for:

```text
Quiz Listing
Quiz Details
Question Display
Random Questions
Timer
Navigation
Submission
Score Calculation
```

---

## Team Member 4 — Teacher Module

Responsible for:

```text
Teacher Dashboard
Create Quiz
Edit Quiz
Question Management
Quiz Management
Teacher Analytics
```

---

## Team Member 5 — Admin Module

Responsible for:

```text
Admin Dashboard
Student Management
Teacher Management
Language Management
Quiz Management
Question Management
Analytics
```

---

## Team Member 6 — Results / Leaderboard

Responsible for:

```text
Result Page
Answer Review
Attempt History
Performance
Leaderboard
Statistics
```

If the team has fewer members, combine related modules.

---

# 47. Testing Requirements

Every feature must be tested before merging.

## Student Testing

Test:

```text
Registration
Login
Logout
Language Selection
Difficulty Selection
Quiz Start
Question Navigation
Timer
Answer Selection
Quiz Submission
Result
Answer Review
Attempt History
```

## Teacher Testing

Test:

```text
Registration
Login
Approval
Create Quiz
Edit Quiz
Delete Quiz
Add Question
Edit Question
Delete Question
View Results
```

## Admin Testing

Test:

```text
Login
Student Management
Teacher Management
Language Management
Quiz Management
Question Management
Analytics
```

---

# 48. Error Handling

The application should properly handle:

```text
Invalid Login
Invalid Registration
Missing Fields
Invalid Quiz
No Questions Available
Quiz Expiration
Unauthorized Access
Invalid URL
Database Errors
```

Do not expose sensitive technical information to normal users.

---

# 49. Security Requirements

Students should not be able to access teacher/admin pages.

Teachers should not be able to access admin functionality.

Admin functionality should be protected.

Users should only be able to modify data they are authorized to modify.

Do not store passwords as plain text.

Use Django's authentication/password hashing system.

---

# 50. Responsive Requirements

The website should work on:

```text
Desktop
Laptop
Tablet
Mobile
```

Test at multiple screen sizes.

Important pages:

```text
Homepage
Login
Registration
Student Dashboard
Quiz Page
Result Page
Teacher Dashboard
Admin Dashboard
```

---

# 51. Project Development Phases

## Phase 1 — Existing System Analysis

* Understand existing Django project
* Understand models
* Understand URLs
* Understand views
* Understand templates
* Run existing application
* Document existing functionality

---

## Phase 2 — UI Redesign

* New branding
* Navbar
* Homepage
* Footer
* Programming categories
* Responsive layout
* Images
* Animations

---

## Phase 3 — Programming Categories

* Language management
* Language pages
* Difficulty levels
* Quiz listing

---

## Phase 4 — Student Module

* Student dashboard
* Profile
* Language selection
* Quiz selection
* Attempt history
* Progress

---

## Phase 5 — Quiz Engine

* Question display
* MCQ
* Code-output questions
* True/False
* Timer
* Random questions
* Navigation
* Submission

---

## Phase 6 — Results

* Score
* Percentage
* Pass/fail
* Correct answers
* Incorrect answers
* Answer review
* Explanation
* Attempt history

---

## Phase 7 — Teacher

* Teacher dashboard
* Quiz creation
* Question creation
* Quiz management
* Question management
* Performance analytics

---

## Phase 8 — Admin

* Admin dashboard
* User management
* Teacher approval
* Language management
* Quiz management
* Question management
* Analytics

---

## Phase 9 — Leaderboard

* Overall ranking
* Language ranking
* Quiz ranking
* Weekly/monthly ranking if approved

---

## Phase 10 — Final Testing

* Functional testing
* UI testing
* Responsive testing
* Authentication testing
* Database testing
* Security testing
* Cross-module testing

---

# 52. Definition of Done

A module is considered complete only when:

* Feature is implemented
* Existing related functionality still works
* Database changes have migrations
* URLs work
* Forms validate correctly
* Unauthorized access is prevented
* UI is responsive
* Errors are handled
* Feature has been manually tested
* Code is committed to Git
* Branch is pushed
* Pull request is ready for review

---

# 53. Final Expected System

The final application should provide:

```text
                    PROGRAMMING QUIZ PLATFORM

        ┌──────────────────────────────────────────┐
        │                 HOME                     │
        └────────────────────┬─────────────────────┘
                             │
              ┌──────────────┼──────────────┐
              │              │              │
           STUDENT        TEACHER         ADMIN
              │              │              │
         Dashboard       Dashboard      Dashboard
              │              │              │
        Languages        Quizzes        Users
              │              │              │
        Difficulty       Questions      Languages
              │              │              │
           Quizzes       Analytics      Quizzes
              │                             │
            Quiz                         Questions
              │                             │
          Questions                    Analytics
              │
           Result
              │
        Answer Review
              │
        Attempt History
              │
         Performance
              │
         Leaderboard
```

---

# 54. Important Instruction for Students

This is a collaborative development project.

Do not assume that a file can be replaced without checking its dependencies.

Before modifying existing code:

1. Read the file.
2. Understand its purpose.
3. Identify dependencies.
4. Make the smallest required change.
5. Run the project.
6. Test the affected functionality.
7. Commit your changes.
8. Push your branch.
9. Create a Pull Request.
10. Wait for review before merging.

The objective is not simply to add new pages.

The objective is to build a **stable, connected, production-quality Programming Quiz Platform** without breaking the existing Django application.

```

### Recommended assignment structure

For your students, I would divide the work into **modules rather than giving everyone the whole application**:

| Module | Main responsibility |
|---|---|
| Module 1 | UI / Homepage / Navbar / Images / Animations |
| Module 2 | Student registration, login & dashboard |
| Module 3 | Programming languages & difficulty |
| Module 4 | Quiz engine, timer & random questions |
| Module 5 | Results, review & attempt history |
| Module 6 | Teacher dashboard & quiz creation |
| Module 7 | Admin dashboard & management |
| Module 8 | Leaderboard & analytics |
| Module 9 | Testing, responsive design & integration |

This gives you a clear way to assign each student/team a Git branch and then merge their work into the main project.
```
