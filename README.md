<!DOCTYPE html>
<html lang="es">

<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Client Project Request</title>

<link rel="preconnect" href="https://fonts.googleapis.com">

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Poppins;
}

body{

background:
linear-gradient(
135deg,
#020617,
#0f172a,
#1e293b
);

min-height:100vh;

display:flex;

justify-content:center;

align-items:center;

padding:40px;

color:white;

}

.container{

width:100%;
max-width:950px;

background:
rgba(
15,
23,
42,
0.9
);

padding:50px;

border-radius:30px;

backdrop-filter:blur(18px);

box-shadow:
0 0 50px rgba(
56,
189,
248,
0.25
);

}

h1{

font-size:42px;

text-align:center;

color:#38bdf8;

margin-bottom:10px;

}

p{

text-align:center;

margin-bottom:40px;

}

form{

display:grid;

grid-template-columns:
1fr 1fr;

gap:20px;

}

.full{

grid-column:span 2;

}

input,
textarea,
select{

padding:16px;

border:none;

outline:none;

border-radius:15px;

background:#1e293b;

color:white;

}

textarea{

height:160px;

resize:none;

}

button{

grid-column:span 2;

padding:18px;

background:#38bdf8;

border:none;

border-radius:15px;

font-size:18px;

font-weight:700;

cursor:pointer;

}

button:hover{

transform:translateY(-4px);

}

</style>

</head>

<body>

<div class="container">

<h1>

📋 Project Request Form

</h1>

<p>

Complete the form to request a project.

</p>

<form id="clientForm">

<input
type="text"
placeholder="Full Name"
required>

<input
type="email"
placeholder="Email"
required>

<input
type="text"
placeholder="Company">

<select>

<option>Website</option>

<option>Business System</option>

<option>Database</option>

<option>Portfolio</option>

<option>Application</option>

</select>

<input
class="full"
type="number"
placeholder="Estimated Budget">

<input
class="full"
type="date">

<textarea
class="full"
placeholder="Describe your project">
</textarea>

<button>

Send Request

</button>

</form>

</div>

<script>

document
.getElementById(
"clientForm"
)

.addEventListener(

"submit",

function(e){

e.preventDefault();

alert(
"Request sent successfully"
);

}

);

</script>

</body>

</html>
