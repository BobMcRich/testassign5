<script setup>

</script>

<template>
<div class= "hero">
    <div>
        <h1>HeroFilms</h1>
        
        <link rel="icon" type="image/png" href="superhero icon.png">
        <link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
        <style>
            h1 {
                font-family: "Pacifico", cursive;
            }
        </style>
    </div>
    <div>
        <h1>Superhero Movies</h1>
        <h3>This is a superhero movie catalog. In this website, you can find all movies related to superhero films. Movies such Superman, Batman and more can be found in this website</h3>
        
        
        <div>
            <button class="language-btn">English</button>
            <RouterLink to="/register" class="button register">Register</RouterLink>
            <RouterLink to="/login" class="button login">Login</RouterLink>
        </div>

        <h2>Top Rated Movies</h2>
        <div class="movies">
        </div>
        
    </div>
</div>


</template>

<style scoped>

</style>