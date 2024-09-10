---
layout: base
title: Project Planning
description: plan
hide: false
---
# Basic Addition Calculator

## Select two numbers to add:

<form>
  <label for="num1">Number 1:</label>
  <select id="num1">
    <option value="1">1</option>
    <option value="2">2</option>
    <option value="3">3</option>
    <option value="4">4</option>
    <option value="5">5</option>
    <option value="6">6</option>
    <option value="7">7</option>
    <option value="8">8</option>
    <option value="9">9</option>
    <option value="10">10</option>
  </select>

  <label for="num2">Number 2:</label>
  <select id="num2">
    <option value="1">1</option>
    <option value="2">2</option>
    <option value="3">3</option>
    <option value="4">4</option>
    <option value="5">5</option>
    <option value="6">6</option>
    <option value="7">7</option>
    <option value="8">8</option>
    <option value="9">9</option>
    <option value="10">10</option>
  </select>

  <button type="button" onclick="calculateSum()">Add</button>
</form>

<p>Result: <span id="result">0</span></p>

<script>
  function calculateSum() {
    var num1 = parseInt(document.getElementById("num1").value);
    var num2 = parseInt(document.getElementById("num2").value);
    var sum = num1 + num2;
    document.getElementById("result").innerHTML = sum;
  }
</script>
