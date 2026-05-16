# SkillHub 🎓
### Online Platform for Self-Paced Short Courses

> **Final Year Project — BS Computer Science, Virtual University of Pakistan**  
> **Grade Awarded: 4.0 / 4.0 (Maximum Possible Grade | Equivalent to 1.0 in German Grading Scale)**

---

## 🌟 Project Overview

SkillHub is a full-stack Learning Management System (LMS) built with PHP, MySQL, and Bootstrap using a clean MVC architecture. 
It supports three independent user roles — Admin, Instructor, and Student — each with a fully dedicated panel and functionality.
The entire system was designed, developed, tested, and documented individually.

---

## ✨ Features

### 👨‍💼 Admin Panel
- Complete user management for Students and Instructors
- Course approval and activation control
- System analytics dashboard with platform-wide overview
- Instructor verification and account management
- Activate or deactivate any user or course instantly

### 👨‍🏫 Instructor Panel
- Course creation with structured chapter and topic organization
- Study material and resource uploads per topic
- Assignment and quiz generation for enrolled students
- Student progress monitoring and performance tracking
- Certificate generation and issuance for course completion
- Full profile management with photo upload

### 👨‍🎓 Student Panel
- Course browsing and one-click enrollment
- Self-paced lecture viewing with progress tracking
- Assignment submission and quiz attempts with instant feedback
- Certificate download upon course completion
- Personal dashboard showing enrolled courses and completion status

---

## 🛠️ Technology Stack

| Layer | Technology |
|-------|-----------|
| Backend | PHP with PDO |
| Database | MySQL |
| Frontend | HTML5, CSS3, Bootstrap 5, FontAwesome |
| Architecture | MVC (Model-View-Controller) |
| Authentication | Session-based with role management |
| Security | PDO prepared statements, input validation and sanitization |
| Rich Text | RichText editor for course content creation |
| Icons | FontAwesome 4 |

---

## 🏗️ Project Architecture

## 🏗️ Project Architecture

```text
SkillHub/
├── Admin/
│   ├── Action/
│   │   ├── active-course.php          # Course activation
│   │   ├── active-Instructor.php      # Instructor activation
│   │   ├── active-student.php         # Student activation
│   │   └── instructor-add.php         # Add new instructor
│   ├── inc/
│   │   ├── Header.php
│   │   ├── Footer.php
│   │   └── NavBar.php
│   ├── Courses.php                    # Course management view
│   ├── Instructors.php                # Instructor management view
│   ├── Student.php                    # Student management view
│   └── System-Analysis.php            # Analytics dashboard
│
├── Instructor/
│   ├── Action/
│   │   ├── course-add.php             # Create new course
│   │   ├── upload-materials.php       # Upload study materials
│   │   ├── create-content.php         # Create lecture content
│   │   ├── course-chapter-add.php     # Add chapters
│   │   ├── course-topic-add.php       # Add topics
│   │   └── load-chapters.php          # Load chapter list
│   ├── inc/
│   │   ├── Header.php
│   │   ├── Footer.php
│   │   ├── NavBar.php
│   │   └── Profile.php
│   ├── Courses.php                    # Course listing
│   ├── Courses-add.php                # New course form
│   ├── Courses-content-add.php        # Add lecture content
│   ├── Courses-Materials.php          # Materials management
│   ├── Certificate-Generate.php       # Issue certificates
│   └── Profile-Edit.php               # Edit instructor profile
│
├── Student/
│   └── inc/
│       ├── Header.php
│       ├── Footer.php
│       └── NavBar.php
│
├── Controller/
│   ├── Admin/
│   │   ├── Course.php                 # Course logic
│   │   ├── Instructor.php             # Instructor logic
│   │   ├── Student.php                # Student logic
│   │   └── system.php                 # Analytics logic
│   ├── Instructor/
│   │   ├── Course.php
│   │   ├── CoursesMaterial.php
│   │   └── Instructor.php
│   └── Student/
│       ├── Certificate.php
│       ├── Course.php
│       ├── EnrolledStudent.php
│       └── Student.php
│
├── Models/
│   ├── Course.php                     # Course CRUD operations
│   ├── Student.php                    # Student data management
│   ├── Instructor.php                 # Instructor data management
│   ├── Certificate.php                # Certificate generation logic
│   ├── EnrolledStudent.php            # Enrollment tracking
│   ├── CoursesMaterial.php            # Materials management
│   └── Admin.php                      # Admin operations
│
├── Action/
│   ├── login.php                      # Login handler
│   └── signup.php                     # Registration handler
│
├── Utils/
│   ├── Util.php                       # Helper functions
│   └── Validation.php                 # Input validation and sanitization
│
├── Assets/
│   ├── css/                           # Bootstrap 5, FontAwesome, custom styles
│   ├── js/                            # jQuery, jsPDF, custom scripts
│   ├── fonts/                         # FontAwesome fonts
│   └── img/                           # Images, logo, signatures
│
├── Database_sample.php                # Sample database configuration
├── index.php                          # Landing page
├── login.php                          # Login page
├── signup.php                         # Registration page
├── about.php                          # About page
├── certificate.php                    # Public certificate verification
└── 404.php                            # Custom error page
```
