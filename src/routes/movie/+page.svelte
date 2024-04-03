<style>
    :root {
    --primary-color: rgb(0, 96, 160);
    --secodary-color: rgb(0, 255, 221);
}

* {
    box-sizing:  border-box;
}

main {
    display: flex;
    flex-wrap: wrap;
}

body{
    background-color:  var(--primary-color);
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin: 0;
}

header {
    padding: 10px;
    display: flex;
    justify-content: flex-end;
    background-color: var(--secodary-color);
}

.search {
    background-color: transparent;
    border: 2px solid var(--primary-color);
    border-radius: 50px;
    font-family: inherit;
    font-size: 14px;
    padding: 200px 10px;
}

.search::placeholder {
    color: wheat;
}

.search.search:focus{
    outline: none;
    background-color: rgb(255, 0, 0);
}

.movie {
    width: 800px;
    margin: 10px;
    background-color: var(--secodary-color);
    box-shadow: 0 4px 5px rgba(0, 0, 0, 0.2);
    position: relative;
    overflow: hidden;
    border-radius: 3px;
}

.movie img{
    width: 100%;
}

.movie-info {
    color: rgb(80, 0, 0);
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 20px 30px 30px;
    letter-spacing: 0.5px;
}

.movie-info h3{
    margin-top: 0;
}

.movie-info span{
    background-color: var(--primary-color);
    padding: 25px 5px;
    border-radius: 3px;
    font-weight: bold;
}

.movie-info span.green{
    color: lightseagreen;
}

.overview {
    background-color: white;
    padding: 20px;
    position: absolute;
    left: 0;
    bottom: 0;
    right: 0;
    max-width: 100%;
    transform: translateY(101%);
    transition: transform 0.3s ease-in;
}

.movie:hover .overview{
    transform: translateY(0)
}
</style>

<main id="main">
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Мохаммед Али: История от и до</h3>
            <span class="green">8.3</span>
        </div>
        <div class="overview">
            <h3 id="Description">1996,биографический,документальный,спорт,США</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Малышка на миллион</h3>
            <span class="green">7.8</span>
        </div>
        <div class="overview">
            <h3 id="Description">2004,драма,спорт,США,12+</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Рокки</h3>
            <span class="green">8.1</span>
        </div>
        <div class="overview">
            <h3 id="Description">1976,драма,спорт,США</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Нокдаун</h3>
            <span class="green">8.4</span>
        </div>
        <div class="overview">
            <h3 id="Description">2005,биографический,драма,исторический,США</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Боец</h3>
            <span class="green">7.8</span>
        </div>
        <div class="overview">
            <h3 id="Description">2010,биографический,драма,спорт,США</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Ураган</h3>
            <span class="green">7.6</span>
        </div>
        <div class="overview">
            <h3 id="Description">1999,биографический,драма,спорт,США</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Тайсон</h3>
            <span class="green">7.4</span>
        </div>
        <div class="overview">
            <h3 id="Description">2008,документальный,США</h3>
        </div>
    </div>
</main>