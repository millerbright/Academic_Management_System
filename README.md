# **Academic Management System - Hệ thống quản lý học thuật - LMS**

## 📌 **Introduction**

🎓 With the aim of creating a high-quality learning environment alongside the development of information technology, a software system has been designed to serve as a comprehensive academic management platform. This software provides a variety of conveniences for students and teachers while also acting as an effective interaction platform between students, teachers, and the school. With separate login functions for lecturers and students, the system ensures data security and easy access to necessary information. Additionally, the software offers a user-friendly interface that is easy for everyone to use.

🎓 In the lecturer login sessions, users have the right to access and manage student information. Lecturers can also manage their personal information, degrees, and expertise. The software provides lecturers with the ability to update course content and support student competency assessment through quizzes.

🎓 With the student login function, users can manage their personal information. Furthermore, they have access to their academic progress and grades. The software also enables students to register for or withdraw from courses. To ensure data security, the system only allows users to view their own personal information and grades, preventing access to other students' data.

## 🛠️ **Technologies Used**

🔧 Frontend: HTML, CSS, JavaScript

🔧 Backend: Spring Boot (Java)

🔧 Database: Google Firebase (Firestore, Firebase Storage)

🔧 Security: Spring Security, JWT Authentication

## 🚀 **Source code:**
The source code of the software can be accessed via the following link:

🔗 [Academic Management System](https://github.com/NguyenVu04/BTL.git)

## 📺 **Video Introduction:**
Product introduction video:

🔗 [Academic Management System](https://youtu.be/HpA0xAE15ZE?si=Bu4EhRuMUR9bwU4F)

## 📌**Software Design - Thiết kế phần mềm** 
The software is designed as a web application and is divided into two main parts: `frontend` and `backend`.
### Frontend: 
The frontend is built using HTML, CSS, and JavaScript.
- HTML (Hypertext Markup Language) is a markup language used to create web pages.
- CSS (Cascading Style Sheets) helps style web elements, making them more dynamic and visually appealing.
- JavaScript is a programming language that enables user interaction with the website.

### Backend: 
The backend is implemented using Spring Boot, a Java framework that facilitates web development by providing various built-in features. It is responsible for storing and processing data as well as handling the infrastructure needed for the application to function.

The **`backend`** structure is organized into the following packages and components:
- `model` package: Contains the abstract class `Model`, which is inherited by the `Course`, `Student`, and `Teacher` classes.
- `Course` package: Includes:
  - `Course` class: Stores course-related information.
  - `NameIDStu` class: Stores student results and details related to a specific course.
- `Student` package: Includes:
  - `Student` class: Stores student information.
  - `Gender` class: Stores student gender details.
- `Teacher` package: Includes:
  - `Certificate` class: Represents the certifications and degrees of lecturers.
  - `Teacher` class: Stores lecturer information.
- `QuizMain` package: Enhances the effectiveness of student assessments, allowing lecturers to create online quizzes easily.
- `firebase` package: Integrates Google Firebase as the database.
- `repository` package: Contains:
  - `BackendStorage` and `FirestoreRepository` classes: Handle interactions with Firebase Storage and Firestore Database.
- `security` package: Implements Spring Security authentication mechanisms. It includes the following classes:
  - `JwtAuthenticationFilter`: Defines a filter to process JWT-based authentication requests.
  - `UserRole`: Defines user roles and privileges in the system.
  - `BackendSecurityConfiguration`: Configures JWT authentication filtering and authentication mechanisms for the backend.
  - `BackendDetailsService`: Provides services such as retrieving user information for database interactions.
  - `JwtUtils`: Contains functions for handling JWT tokens (encoding, decoding, extracting data, etc.).
  - `BackendAuthenticationProvider`: Implements an authentication mechanism using email and password.
  - `AuthenticationDetails`: Defines the authentication data structure stored in the database.
The system uses JWT (JSON Web Token) for encryption and authentication.
- `exceptionhandler` package: Handles system exceptions.
- `controller` package:
  - Handles requests from the frontend and returns corresponding responses.
  - Processes user actions, such as login requests, course registrations, and quiz submissions.
  - Includes the following controllers:
      - `AuthenticationController`: Handles login, registration, and authentication.
      - `TeacherController`: Manages lecturer-related operations (view, update, delete information).
      - `StudentController`: Manages student-related operations (view, update, delete information).
      - `QuizController`: Manages quiz-related tasks (adding, modifying questions, creating quizzes, grading, viewing scores, etc.).
      - `CourseController`: Handles course-related actions (adding/removing lecturers and students, updating course content, viewing scores, adding materials and lectures).

**`Frontend Structure`**
The frontend consists of the graphical user interface (GUI) that users interact with. It is stored in the fe directory, which contains the following HTML files:
- `course-detail.html`: Displays course details, including general information, announcements, lecture slides, reference materials, and quizzes.
- `course-score.html`: Displays student scores (for students only), including grade tables and progress tracking.
- `courses.html`: Lists enrolled courses, allowing students to register for new courses or drop existing ones using buttons.
- `index.html`: The homepage, featuring an image carousel and general school information.
- `list_stu.html`: Displays the class list for a specific course.
- `login.html`: Handles user login and registration. It supports separate login options for lecturers and students, requiring email and password authentication.
- `quiz.html`: Enables lecturers to create and manage quizzes for students.
- `student-info.html`: Displays student personal information and provides options for editing personal details.
- `teacher_classlist.html`: Lists the classes assigned to a lecturer.
- `teacher_evaluate.html`: Allows lecturers to update student grades and provide evaluations.
- `teacher_host.html`: Stores and updates lecturer information.
- `teacher-info.html`: Displays a list of all lecturers in the institution.
- `teacher_lich.html`: Shows the lecturer's teaching schedule. Users can adjust the display mode for better viewing.
- `assets` folder:
  - Stores CSS, JavaScript, images, and other design-related files.
  - Enhances the visual appearance and user interactions (fonts, navigation menus, buttons, images, graphs).
This detailed structure ensures that the academic management system is well-organized and functional, providing secure and efficient interactions between students, lecturers, and the institution.
## 🏆 Contributors
1. Võ Quang Đại Việt - 2213954
2. Nguyễn Đình Đức - 2210794
3. Nguyễn Duy Vũ - 2213997
4. Trần Huy Đức - 2210812
5. Chế Minh Đức - 2210783
6. Khúc Minh Trí - 2213636
7. Nguyễn Quang Sáng - 2212922



