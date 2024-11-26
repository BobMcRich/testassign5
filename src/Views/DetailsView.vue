<script setup>
import axios from "axios";
import { useRoute } from "vue-router";

const route = useRoute();
const response = await axios.get(`https://api.themoviedb.org/3/movie/${route.params.id}?api_key=${import.meta.env.VITE_TMDB_KEY}&append_to_response=videos`);
console.log(response.data);
</script>

<template>
<div>
    <div></div>
        <title>HeroFilms</title>
        <link rel="stylesheet" type="text/css" href="style.css">
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
            <button>Sign In</button>
            <button>Sign Out</button>
        </div>

        <h2>Top Rated Movies</h2>
        <div class="movies">

        </div>
        
        <footer>
            <p>HeroFilms, 2024</p>
        </footer>
</div>
</template>

<style scoped>
.movie-detail {
  padding: 20px;
  color: white;
  background-color: #141414; /* Dark background for the detail view */
}

.movie-title {
  font-size: 2.5rem;
  margin-bottom: 10px;
  color: #e50914; /* Netflix red */
}

.movie-overview {
  font-size: 1.2rem;
  margin-bottom: 10px;
}

.movie-release-date {
  font-size: 1rem;
  margin-bottom: 20px;
}

.movie-site {
  display: inline-block;
  margin-bottom: 20px;
  padding: 10px 15px;
  background-color: #e50914; /* Netflix red */
  color: white;
  text-decoration: none;
  border-radius: 5px;
}

.movie-site:hover {
  background-color: #f01212; /* Darker red on hover */
}

.movie-poster {
  width: 25%;
  border-radius: 10px;
  margin-bottom: 20px;
}

.trailers-title {
  font-size: 2rem;
  margin-top: 40px;
  margin-bottom: 20px;
  text-align: center;
}

.trailers-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 15px; /* Space between trailer tiles */
}

.trailer-tile {
  background-color: #222;
  border-radius: 10px;
  overflow: hidden;
  transition: transform 0.2s;
  width: 200px; /* Fixed width for trailer tiles */
}

.trailer-tile:hover {
  transform: scale(1.05); /* Scale effect on hover */
}

.trailer-thumbnail {
  width: 100%; /* Full width of the tile */
  height: auto; /* Maintain aspect ratio */
}
</style>