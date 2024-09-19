---
layout: page
title: About
permalink: /about/
---

# 🌏 My Journey

<div style="display: flex; justify-content: center; align-items: center; gap: 20px; padding: 20px; background-color: #f0f8ff; border-radius: 10px;">
    <img src="https://upload.wikimedia.org/wikipedia/en/thumb/4/41/Flag_of_India.svg/1200px-Flag_of_India.svg.png" alt="India Flag" width="150" />
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a9/Flag_of_the_United_States_%28DoS_ECA_Color_Standard%29.svg/255px-Flag_of_the_United_States_%28DoS_ECA_Color_Standard%29.svg.png" alt="USA Flag" width="150" />
    <img src="https://www.civitatis.com/blog/wp-content/uploads/2022/10/que-ver-san-diego.jpg" alt="San Diego" width="150" />
</div>

Born in **India** 🇮🇳, moved to **San Diego, USA** 🇺🇸 in **2012**.

---

## 🎨 My Life

- 🏫 I went to elementary school at **Monterey Ridge Elementary School** in San Diego.
- 🏫 I attended **Oak Valley Middle School**.
- 🥊 I **box** and enjoy **weight lifting**🏋️.
- 🎨 I am learning to **oil paint**.
- 🐕 I enjoy walking my dog **Alo** every morning.
- 📺 I like to watch **MMA** on TV.
- 💻 I'm interested in **computers**, and I have built many of them myself.

---

## 👨‍👩‍👧‍👦 My Family

-🐶 I have a dog named **Alo**, and we love going on walks every morning.
-👨🏽‍👩🏽‍👧🏽‍👦🏽 I have a younger sister, and we often play video games together.
-⛺ We enjoy **camping**, 🎬 watching **movies**, ♟️ and playing **board games** as a family.

---

## 📸 Family Photo Gallery

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px; padding: 20px; background-color: #f0f8ff; border-radius: 10px;">
    <img src="../images/aranyapic1.jpg" alt="Family Pic 1" style="width: 100%; aspect-ratio: 1/1; object-fit: cover; border-radius: 10px; box-shadow: 0px 4px 8px rgba(0,0,0,0.1);" onclick="openImage(this.src)">
    <img src="../images/aranyapic2.jpg" alt="Family Pic 2" style="width: 100%; aspect-ratio: 1/1; object-fit: cover; border-radius: 10px; box-shadow: 0px 4px 8px rgba(0,0,0,0.1);" onclick="openImage(this.src)">
    <img src="../images/aranya4.jpg" alt="Family Pic 3" style="width: 100%; aspect-ratio: 1/1; object-fit: cover; border-radius: 10px; box-shadow: 0px 4px 8px rgba(0,0,0,0.1);" onclick="openImage(this.src)">
    <img src="../images/aranya5.jpg" alt="Family Pic 4" style="width: 100%; aspect-ratio: 1/1; object-fit: cover; border-radius: 10px; box-shadow: 0px 4px 8px rgba(0,0,0,0.1);" onclick="openImage(this.src)">
    <img src="../images/dogg2.jpg" alt="Dog Pic" style="width: 100%; aspect-ratio: 1/1; object-fit: cover; border-radius: 10px; box-shadow: 0px 4px 8px rgba(0,0,0,0.1);" onclick="openImage(this.src)">
    <img src="../images/guac.jpg" alt="Fun Pic" style="width: 100%; aspect-ratio: 1/1; object-fit: cover; border-radius: 10px; box-shadow: 0px 4px 8px rgba(0,0,0,0.1);" onclick="openImage(this.src)">
</div>

<!-- Full-screen overlay HTML -->
<div id="fullScreenOverlay" class="full-screen-overlay">
  <span class="close-btn" onclick="closeImage()">&times;</span>
  <img id="fullScreenImage" src="" alt="Full Screen">
</div>

<!-- Add this to your head or inside a <style> tag -->
<style>
  /* Styles for full-screen image view */
  .full-screen-overlay {
    display: none;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.8);
    justify-content: center;
    align-items: center;
    z-index: 9999;
  }

  .full-screen-overlay img {
    max-width: 90%;
    max-height: 90%;
    border-radius: 10px;
    box-shadow: 0px 4px 8px rgba(255, 255, 255, 0.5);
  }

  .full-screen-overlay .close-btn {
    position: absolute;
    top: 20px;
    right: 20px;
    font-size: 24px;
    color: white;
    cursor: pointer;
  }

  /* Styling for the quiz */
  .quiz-container {
    margin-top: 50px;
    padding: 20px;
    background-color: #e0f7fa;
    border-radius: 10px;
    box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
  }

  .quiz-container h2 {
    color: #00796b;
  }

  .quiz-container p {
    color: #004d40;
    font-weight: bold;
  }

  .quiz-container label {
    font-weight: normal;
    color: #004d40;
  }

  .quiz-container button {
    margin-top: 20px;
    padding: 10px 20px;
    background-color: #00796b;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
  }

  .quiz-container button:hover {
    background-color: #004d40;
  }

  #quizResult {
    margin-top: 20px;
    font-size: 16px;
    color: #00796b;
  }
</style>

<!-- Add this JavaScript at the bottom -->
<script>
  function openImage(src) {
    document.getElementById('fullScreenImage').src = src;
    document.getElementById('fullScreenOverlay').style.display = 'flex';
  }

  function closeImage() {
    document.getElementById('fullScreenOverlay').style.display = 'none';
  }
</script>

---

## 📝 Quiz About Me

<h2>Quiz About Me</h2>
<p>Test your knowledge with this quick quiz!</p>

<form id="quizForm">
  <p><strong>1. In which year did I move to San Diego?</strong></p>
  <input type="radio" id="q1a" name="q1" value="2010">
  <label for="q1a">2010</label><br>
  <input type="radio" id="q1b" name="q1" value="2012">
  <label for="q1b">2012</label><br>
  <input type="radio" id="q1c" name="q1" value="2014">
  <label for="q1c">2014</label><br>

  <p><strong>2. What is the name of my dog?</strong></p>
  <input type="radio" id="q2a" name="q2" value="Alo">
  <label for="q2a">Alo</label><br>
  <input type="radio" id="q2b" name="q2" value="Max">
  <label for="q2b">Max</label><br>
  <input type="radio" id="q2c" name="q2" value="Rex">
  <label for="q2c">Rex</label><br>

  <p><strong>3. Which sport do I enjoy watching on TV?</strong></p>
  <input type="radio" id="q3a" name="q3" value="Football">
  <label for="q3a">Football</label><br>
  <input type="radio" id="q3b" name="q3" value="MMA">
  <label for="q3b">MMA</label><br>
  <input type="radio" id="q3c" name="q3" value="Basketball">
  <label for="q3c">Basketball</label><br>

  <p><strong>4. What is one of my hobbies?</strong></p>
  <input type="radio" id="q4a" name="q4" value="Cooking">
  <label for="q4a">Cooking</label><br>
  <input type="radio" id="q4b" name="q4" value="Oil painting">
  <label for="q4b">Oil painting</label><br>
  <input type="radio" id="q4c" name="q4" value="Skiing">
  <label for="q4c">Skiing</label><br>

  <p><strong>5. Which school did I attend for middle school?</strong></p>
  <input type="radio" id="q5a" name="q5" value="Monterey Ridge Elementary">
  <label for="q5a">Monterey Ridge Elementary</label><br>
  <input type="radio" id="q5b" name="q5" value="Oak Valley Middle School">
  <label for="q5b">Oak Valley Middle School</label><br>
  <input type="radio" id="q5c" name="q5" value="Poway High School">
  <label for="q5c">Poway High School</label><br>

  <button type="button" onclick="checkQuiz()" style="margin-top: 20px; padding: 10px 20px; background-color: #00796b; color: white; border: none; border-radius: 5px; cursor: pointer;">Submit Quiz</button>
</form>

<p id="quizResult"></p>

<script>
  function checkQuiz() {
    var score = 0;
    var totalQuestions = 5;

    // Check answers
    if (document.querySelector('input[name="q1"]:checked')?.value === '2012') score++;
    if (document.querySelector('input[name="q2"]:checked')?.value === 'Alo') score++;
    if (document.querySelector('input[name="q3"]:checked')?.value === 'MMA') score++;
    if (document.querySelector('input[name="q4"]:checked')?.value === 'Oil painting') score++;
    if (document.querySelector('input[name="q5"]:checked')?.value === 'Oak Valley Middle School') score++;

    // Display result
    document.getElementById('quizResult').innerText = 'You scored ' + score + ' out of ' + totalQuestions + '.';
  }
</script>
<body>
<script src="https://utteranc.es/client.js"
        repo="Mom5MoreMins/aranya_student_2025"
        issue-term="pathname"
        theme="github-dark"
        crossorigin="anonymous"
        async>
    </script>
</body>
