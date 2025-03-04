---
layout: base
title: API Model: How It Works
permalink: /blog/api-model
menu: nav/blog.html
---
# Retrospective: Trimester 2

## 1. National Parks Personality Quiz
![Insert Image Here](./cspblog/quizsuccess.png)

The **National Parks Personality Quiz** helps users determine which national park best matches their interests. By answering a series of questions, users receive a personalized recommendation, making it an engaging and educational feature of our website.

## 2. Planning and Personal Contribution Video
![Watch Planning Video](./cspblog/frostbyte_vid.mp4)


The **Planning and Personal Contribution Video** was created to establish a clear vision for our project. My role was crucial in **editing and piecing together the video** to ensure it effectively communicated our goals and team contributions.

## 3. Camping Homepage
![Insert Image Here](./cspblog/homepage.png)

I developed the **Camping Homepage**, which serves as an introduction to the camping side of our website. This page features a **slideshow of national park images**, allowing users to **fullscreen images with a single click**, making it an interactive and visually appealing experience.

## 4. Styling the Camping Side

One of my major contributions was **styling the entire camping section** of our project. This directly addressed the criticism we received at **Night at the Museum**, where our project was called "gray." I improved the aesthetics to enhance user engagement and appeal.

## 5. Assistant Deployment Manager

As **Assistant Deployment Manager**, I played a key role in resolving **bugs and errors**, such as **CORS errors**, before my teammates contributed to the deployed site. My work ensured a **smooth deployment process** and minimized technical roadblocks for our team.

---
## Demo: National Park Personality Quiz
![Watch Planning Video](./cspblog/bruh.mp4)

Click the image above to watch a **video demo** of the National Park Personality Quiz in action.

---

## CPT Requirements Table

| CPT Requirements              | Example Code Snippet |
|--------------------------------|---------------------------|
| Use of at least one list (or other collection type) to represent a collection of data that is stored and used to manage program complexity and help fulfill the program’s purpose | ```python sample_results = [ {"user_id": 1, "assigned_park": "Denali National Park"}, {"user_id": 2, "assigned_park": "Grand Canyon National Park"} ] ``` (From `initQuizResults` function in `QuizResult` model) |
| At least one procedure that contributes to the program’s intended purpose, where you have defined: the procedure’s name, the return type, one or more parameters | ```python def assign_national_park(self, total_points): ``` (From `_CRUD` class in `QuizAPI`) |
| Algorithm that includes sequencing, selection, and iteration that is in the body of the selected procedure | ```python if 0 <= total_points <= 130: return "Denali National Park" elif 140 <= total_points <= 170: return "Grand Canyon National Park" ``` (From `assign_national_park` function in `QuizAPI`) |
| Calls to your student-developed procedure | ```python assigned_park = self.assign_national_park(total_points) ``` (From `post` method in `QuizAPI`) |
| Instructions for output | ```javascript document.getElementById("result").innerText = `✅ Quiz Submitted Successfully! Total Points: ${total_points} Assigned Park: ${data.assigned_park || "Unknown"}`; ``` (From `submitQuiz()` function in frontend JavaScript) |

---

### Explanation of CPT Requirements in the Project

The **National Parks Personality Quiz** satisfies all **College Board CPT** requirements by utilizing key programming concepts:

1. **List/Data Collection**: The backend stores user quiz results in a database and uses lists (`sample_results`) for initialization.
2. **Procedures with Parameters**: The function `assign_national_park(total_points)` determines the appropriate national park based on a user's quiz score.
3. **Algorithm with Control Flow**: The function contains **sequencing, selection, and iteration** to evaluate user points and return a corresponding national park.
4. **Procedure Calls**: The `assign_national_park` function is called within the `post` method to assign a national park dynamically.
5. **Output Instructions**: The frontend JavaScript dynamically displays the quiz result on-screen, providing users with immediate feedback.

These components work together to create a **fully functional, interactive quiz** that assigns users a national park based on their preferences. The project meets **AP CSP CPT** standards while demonstrating real-world software development concepts.
