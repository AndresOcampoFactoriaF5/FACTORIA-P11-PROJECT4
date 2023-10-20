<script>
    const url = 'https://api.themoviedb.org/3/discover/movie?include_adult=false&include_video=false&language=es-ES&page=1&sort_by=popularity.desc'
    const options = {
  method: 'GET',
  headers: {
    accept: 'application/json',
    Authorization: 'Bearer eyJhbGciOiJIUzI1NiJ9.eyJhdWQiOiI0MTEwNjgwYWY3MDMzYjEzNDVhZmZmOGY2ZTM2NjA2NCIsInN1YiI6IjY1MzBmM2JkMTEwOGE4MDE0ZDM1NmFhYiIsInNjb3BlcyI6WyJhcGlfcmVhZCJdLCJ2ZXJzaW9uIjoxfQ.YEGZWMDekCm8L8bAFB2J--DyoSfjGJz5d7j8NSV9ui8'
  }
};

let movies = [];

    fetch(url, options)
        .then((response) => response.json())
        .then( data => movies = data.results)
        .catch((err) => console.error(err));

</script>    

<div>
    {#each movies as movie }
    <img
        alt="cover"
        src={"https://image.tmdb.org/t/p/original/" + movie.poster_path}>
    {/each }
    
</div>

