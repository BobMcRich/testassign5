<script setup>

</script>

<template>

</template>

<style scoped>
body{
  background-color: aqua;
}
.header {
position: fixed;
top: 0;
left: 0;
width: 100%;
background: rgba(0, 0, 0, 0.7);
padding: 10px 20px;
z-index: 100;
}
h1 {
font-family: "Pacifico", cursive;
text-align: center;
margin-top: 20px;
}
h2 {
text-align: left;
margin: 20px 0 10px 0;
}

h3 {
text-align: center;
color: gold;
margin: 10px 0;
}

p {
color: black;
text-align: center;
margin: 10px 0;
}

.movies {
display: flex;
justify-content: center;
flex-wrap: wrap;
gap: 2%;
margin: 100px 0 20px;
}
.movies img {
border: 3px solid red;
width: 200px;
height: auto;
object-fit: cover;
transition: opacity 0.3s ease, transform 0.3s ease;
}
.movies img:hover {
opacity: 0.8;

transform: scale(1.05);
}
.button-container {
text-align: center;
margin: 0;
}
.language-btn {
margin-right: 10px;
padding: 10px 20px;
background-color: #ffcc00;
border: none;
border-radius: 5px;
cursor: pointer;
font-weight: bold;
transition: background-color 0.3s;
}
.language-btn:hover {
background-color: #ff9900;
}
footer {
text-align: center;
margin: 20px 0;
z-index: 2;
</style>
