Yes. Since students will **pull the repository, modify the HTML/CSS/JS, and push their work**, the README should clearly state the current baseline and the rules.

You can use this as the project's `README.md`:

````markdown
# 5-Throne's Programming Quiz

A Django-based Programming Quiz Platform developed as a collaborative frontend enhancement project.

The project is based on an existing Django Online Quiz system. The current backend workflow is preserved so that students can focus on improving and rebuilding the frontend interface.

---

## Project Status

### Current Version

**Version:** 1.0 - Base Django Quiz System

### Current Status

The project currently contains the complete basic Django structure for:

- Home page
- Student module
- Teacher module
- Admin module
- Quiz module
- Course management
- Question management
- Student examinations
- Result calculation
- Student marks
- Teacher management
- Admin management
- Authentication

The existing Django backend, database models, views, forms, URLs and migrations are being preserved.

The next phase of development is focused mainly on **frontend redesign and UI/UX enhancement**.

---

# Existing Project Structure

```text
Programming-Quiz/
│
├── manage.py
│
├── onlinequiz/
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
│
├── quiz/
│   ├── models.py
│   ├── views.py
│   ├── forms.py
│   ├── urls.py
│   └── migrations/
│
├── student/
│   ├── models.py
│   ├── views.py
│   ├── forms.py
│   ├── urls.py
│   └── migrations/
│
├── teacher/
│   ├── models.py
│   ├── views.py
│   ├── forms.py
│   ├── urls.py
│   └── migrations/
│
├── templates/
│   ├── quiz/
│   ├── student/
│   └── teacher/
│
├── static/
│
├── db.sqlite3
│
└── requirements.txt
````

---

# Main Objective

Transform the existing Online Quiz application into a professional:

**5-Throne's Programming Quiz Platform**

The backend functionality should remain stable while the frontend interface is redesigned.

---

# Student Work

Students are mainly responsible for the frontend interface.

Students should work on:

* HTML
* CSS
* JavaScript
* UI/UX
* Responsive design
* Animations
* Images
* Video backgrounds
* Cards
* Navigation
* Buttons
* Forms
* Dashboard layouts
* Quiz interface
* Result interface

---

# Important Rule

## Do Not Modify Backend Files Without Permission

The following files and folders should not be changed unless specifically assigned:

```text
*.py
```

Especially:

```text
models.py
views.py
forms.py
urls.py
settings.py
```

Do not modify:

```text
migrations/
```

Do not delete:

```text
db.sqlite3
```

Do not change the database structure unless specifically instructed.

---

# HTML Work

The main frontend work will be inside:

```text
templates/
```

Structure:

```text
templates/
│
├── quiz/
│
├── student/
│
└── teacher/
```

Students may redesign the HTML interfaces inside these folders.

---

# Home Page

The Home page should be redesigned into a professional programming-focused landing page.

Required sections:

```text
Navbar
↓
Hero Section
↓
Programming Quiz Introduction
↓
Programming Categories
↓
Featured Quizzes
↓
How It Works
↓
Call To Action
↓
Footer
```

The Hero section should support:

* 3D visual or video background
* Programming theme
* 5-Throne's branding
* Strong heading
* Short description
* Start Quiz / Student Signup button

The provided 10-second video should:

* Autoplay
* Loop continuously
* Remain muted
* Work on desktop and mobile
* Use `playsinline`

---

# Student Module

The Student interface should eventually contain:

```text
Student Login
        ↓
Student Signup
        ↓
Student Dashboard
        ↓
Available Programming Quizzes
        ↓
Quiz Instructions
        ↓
Start Quiz
        ↓
Questions
        ↓
Submit Quiz
        ↓
Result
        ↓
Marks / Performance
```

Students should improve the visual design without breaking the existing Django workflow.

---

# Teacher Module

The Teacher interface should contain:

```text
Teacher Login
        ↓
Teacher Signup
        ↓
Teacher Dashboard
        ↓
Manage Courses
        ↓
Create Exam
        ↓
Add Questions
        ↓
View Questions
        ↓
Manage Exams
```

Students should improve the UI while preserving the existing functionality.

---

# Admin Module

The Admin interface should eventually provide:

```text
Admin Login
        ↓
Admin Dashboard
        ↓
Students
        ↓
Teachers
        ↓
Courses
        ↓
Questions
        ↓
Student Marks
        ↓
Teacher Management
        ↓
Reports
```

The admin functionality already exists in the backend.

The frontend should be redesigned professionally.

---

# Design Requirements

The new interface should be:

* Professional
* Modern
* Responsive
* Clean
* Attractive
* Programming focused
* Consistent across all pages
* Desktop friendly
* Mobile friendly

Use a consistent design system for:

* Colors
* Typography
* Buttons
* Cards
* Forms
* Navigation
* Spacing
* Shadows
* Animations

---

# Branding

Project name:

**5-Throne's Programming Quiz**

The interface should use consistent branding throughout:

```text
5-Throne's
Programming Quiz
```

Avoid using the old generic:

```text
Online Quiz
```

where the new branding is appropriate.

---

# No Emojis

Do not add emojis to the interface unless explicitly requested.

Use professional UI elements, icons, typography, animations and visual components instead.

---

# Collaboration Rules

Each student must:

1. Clone the repository.
2. Create their own branch.
3. Work only on the assigned frontend area.
4. Test the website locally.
5. Commit changes with a meaningful message.
6. Push the branch.
7. Create a Pull Request.
8. Wait for review before merging.

---

# Git Workflow

Clone the repository:

```bash
git clone <REPOSITORY-URL>
```

Enter the project:

```bash
cd Programming-Quiz
```

Create a branch:

```bash
git checkout -b feature/student-dashboard-ui
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the project:

```bash
py manage.py runserver
```

Open:

```text
http://127.0.0.1:8000/
```

---

# Branch Naming

Use meaningful branch names.

Examples:

```text
feature/home-ui
feature/navbar-ui
feature/footer-ui
feature/student-dashboard
feature/student-login
feature/student-quiz-ui
feature/student-result-ui
feature/teacher-dashboard
feature/teacher-exam-ui
feature/admin-dashboard
feature/admin-ui
feature/responsive-design
feature/animations
```

---

# Commit Messages

Use clear commit messages.

Examples:

```bash
git add .
git commit -m "Redesign home page UI"
```

```bash
git commit -m "Improve student dashboard interface"
```

```bash
git commit -m "Add responsive quiz layout"
```

```bash
git commit -m "Update teacher dashboard UI"
```

Avoid messages such as:

```text
update
changes
done
final
test
```

---

# Pull Request Requirements

Before creating a Pull Request, verify:

* Website starts successfully.
* No Django errors.
* No broken links.
* No missing templates.
* No console errors.
* Existing functionality still works.
* UI is responsive.
* No unnecessary files are committed.
* No backend files were changed without permission.

---

# Team Development Areas

The project can be divided into the following teams:

## Team 1 - Home Page

Responsible for:

```text
index.html
navbar.html
footer.html
```

## Team 2 - Student UI

Responsible for:

```text
student/
```

Main focus:

* Login
* Signup
* Dashboard
* Quiz selection
* Quiz interface
* Results

## Team 3 - Teacher UI

Responsible for:

```text
teacher/
```

Main focus:

* Login
* Signup
* Dashboard
* Course management
* Exam management
* Question management

## Team 4 - Admin UI

Responsible for:

```text
quiz/admin*.html
```

Main focus:

* Admin login
* Dashboard
* Student management
* Teacher management
* Course management
* Question management
* Marks

## Team 5 - UI/UX & Responsive Design

Responsible for:

* Responsive layouts
* Animations
* Consistent styling
* Mobile optimization
* Accessibility
* Cross-browser testing

---

# Current Development Phase

## Phase 1 - Base Project

Status: Completed

The existing Django quiz application provides the basic backend workflow.

## Phase 2 - Frontend Redesign

Status: In Progress

Main objective:

**Replace the old Online Quiz interface with the new 5-Throne's Programming Quiz interface.**

## Phase 3 - Programming Quiz Enhancement

Planned:

* Programming categories
* Improved quiz interface
* Better result visualization
* Progress indicators
* Performance statistics
* Improved student dashboard

## Phase 4 - Advanced Features

Planned:

* Leaderboard
* Quiz history
* Performance analytics
* Difficulty levels
* Timed quizzes
* Programming topic filtering
* Improved teacher tools
* Improved admin analytics

---

# Development Principle

The most important rule for this project:

> Preserve the existing Django functionality while continuously improving the frontend experience.

Backend first.

Frontend enhancement second.

Test before merging.

---

# Project Goal

The final application should become a complete programming learning and assessment platform where students can:

* Learn programming concepts
* Practice questions
* Take programming quizzes
* View results
* Track performance
* Improve their skills

Teachers should be able to:

* Create courses
* Create quizzes
* Add questions
* Manage exams
* Review student performance

Administrators should be able to:

* Manage students
* Manage teachers
* Manage courses
* Manage questions
* Monitor results
* Manage the complete platform

---

# Current Status

**Backend:** Existing Django quiz system preserved

**Database:** Existing database structure preserved

**Student Module:** Existing functionality preserved

**Teacher Module:** Existing functionality preserved

**Admin Module:** Existing functionality preserved

**Quiz Module:** Existing functionality preserved

**Frontend:** Ready for collaborative redesign

**Current Priority:** Build the new 5-Throne's Programming Quiz UI

````

### Recommended repository workflow

Since you're going to have students collaborate, I would make the repository's **main branch the stable base**:

```text
main
  |
  ├── feature/home-ui
  ├── feature/student-ui
  ├── feature/teacher-ui
  ├── feature/admin-ui
  └── feature/quiz-ui
````

Students should **never directly push to `main`**. They push their branch and create a Pull Request. You review it and merge it.

This is especially important because all the frontend pages are connected to the existing Django views.
