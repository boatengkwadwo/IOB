
# WEB101 - Module 1: HTML5 Basics

**HTML = Skeleton of website**

**Your First Website Code:**
```html
<!DOCTYPE html>
<html>
<body style="font-family:Arial; background:#f0f2f5;">
  <h1 style="color:#0d47a1;">Welcome to IOB</h1>
  <p>My name is [Your Name] - IT Student</p>
  <img src="https://via.placeholder.com/200" width="200">
  <br><br>
  <a href="https://google.com">My Facebook</a>
</body>
</html>#

 Module 2: CSS3 Styling - Make it Beautiful

**CSS = Clothing for your website**

**3 Ways to add CSS:**
1. Inline: <p style="color:red">
2. Internal: <style> in head
3. External: link to style.css (BEST)

**Example style.css:**
```css
body {
  font-family: 'Segoe UI', sans-serif;
  background: #f8f9fa;
}
h1 {
  color: #0d47a1;
  text-align: center;
  background: #ffca28;
  padding: 20px;
  border-radius: 10px;
}
.card {
  background: white;
  padding: 20px;
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  border-radius: 10px;
}

# Module 2: CSS3 Styling - Make it Beautiful

**CSS = Clothing for your website**

**3 Ways to add CSS:**
1. Inline: <p style="color:red">
2. Internal: <style> in head
3. External: link to style.css (BEST)

**Example style.css:**
```css
body {
  font-family: 'Segoe UI', sans-serif;
  background: #f8f9fa;
}
h1 {
  color: #0d47a1;
  text-align: center;
  background: #ffca28;
  padding: 20px;
  border-radius: 10px;
}
.card {
  background: white;
  padding: 20px;
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  border-radius: 10px;
}

**FILE: `Web-Technology-1/Module-03.md`**
```md
# Module 3: JavaScript Basics - Make it Interactive

**JS = Brain of website**

**Example - Alert and Calculator:**
```html
<button onclick="greet()">Click Me</button>
<script>
function greet(){
  alert("Welcome to IOB!");
}
function add(){
  var a = parseInt(document.getElementById('num1').value);
  var b = parseInt(document.getElementById('num2').value);
  document.getElementById('result').innerHTML = a + b;
}
</script>

<input id="num1" placeholder="Number 1">
<input id="num2" placeholder="Number 2">
<button onclick="add()">Add</button>
<p id="result"></p>

Task: Style your Module 1 HTML page with CSS to look like university ID card.
