# Django Online Course - Assessment Feature

## 📌 Project Overview

This project is a full-stack Django web application that extends an online course platform by adding a functional **Exam and Assessment feature**. It allows administrators to create multiple-choice exams for courses and allows learners to take those exams, submit their answers, and immediately see their graded results.

This project was built to practice and demonstrate proficiency in Django's core architecture, including models, views, templates, and the Django admin panel.

## 🚀 Key Features Built

* **Relational Database Design:** Built custom Django models for `Question`, `Choice`, and `Submission` that link directly to existing `Course` and `Enrollment` tables.
* **Custom Admin Dashboard:** Configured the Django Admin interface with `StackedInline` views so administrators can easily create and edit questions and choices directly from the Course page.
* **Dynamic Front-End Templates:** Utilized Django Template Language (DTL) and Bootstrap to dynamically generate exam forms based on the questions stored in the database.
* **Custom Backend Grading Logic:** Engineered view functions to capture `POST` request data, compare selected choices against the correct database answers, calculate total scores, and evaluate Pass/Fail conditions.
* **Interactive Results Page:** Created a styled results dashboard that highlights correct answers, warns about missed correct answers, and flags wrong selections for the user.

## 🧠 What I Learned

Throughout the development of this project, I gained hands-on experience with:

1. **Django ORM & Database Architecture:** Creating complex relational models (Foreign Keys, Many-to-Many fields) and safely migrating schema changes to a local SQLite database.
2. **Django Admin Customization:** Registering models and utilizing `admin.StackedInline` and `admin.ModelAdmin` to create a polished content management experience without writing custom frontend forms.
3. **Backend Logic & Routing:** Writing custom Python views to handle form submissions, process data securely with `{% csrf_token %}`, and routing URLs with dynamic parameters (`<int:course_id>`).
4. **Django Template Language (DTL):** Using `{% for %}` loops and `{% if %}` statements to build dynamic HTML pages that react to backend context variables.
5. **Local Environment Setup:** Setting up Python virtual environments (`venv`), managing dependencies via `requirements.txt`, and resolving package compatibility issues.
6. **Git & GitHub Workflow:** Moving from a cloud-based lab environment to local VS Code development, initializing repositories, writing clean commits, and pushing code using terminal commands.

## 🛠️ Technologies Used

* **Backend:** Python, Django
* **Database:** SQLite
* **Frontend:** HTML, CSS, Bootstrap
* **Version Control:** Git, GitHub
