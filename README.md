<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Palindrome Checker</title>
  <style>
    body {
      font-family: Arial;
      text-align: center;
      margin-top: 50px;
    }
    input, button {
      padding: 10px;
      margin: 5px;
    }
  </style>
</head>
<body>

<h2>Palindrome Checker</h2>

<input type="text" id="text" placeholder="Enter text">
<button onclick="checkPalindrome()">Check</button>

<p id="result"></p>

<script>
function checkPalindrome() {
  let str = document.getElementById("text").value;
  let reversed = str.split("").reverse().join("");

  if(str === reversed) {
    document.getElementById("result").innerText = "Palindrome";
  } else {
    document.getElementById("result").innerText = "Not Palindrome";
  }
}
</script>

</body>
</html>
```
