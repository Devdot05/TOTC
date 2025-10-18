<script>
    let name = "Dotun"
    let age = 22
    let location = "Nigeria"
    let hubby = "programming"
    let simpleHTML = "<h1>This is a simple <b>HTML paragraph</b></h1>"
    const friends = ["Dotun", "Ade", "Bisi", "Bunmi", "Temitope"]
    const movies = [
        { title: "The Godfather", year: 1972, genre: "Crime, Drama" },
        { title: "The Shawshank Redemption", year: 1994, genre: "Drama" },
        { title: "The Dark Knight", year: 2008, genre: "Action, Crime, Drama" },
        { title: "The Lord of the Rings: The Return of the King", year: 2003, genre: "Action, Adventure, Drama" },
        { title: "Pulp Fiction", year: 1994, genre: "Crime, Drama" }
    ]
    let isVissible = $state(true)
    let score = $state(80)
    let hour = $state(20)
</script>
<header class="col-8 mx-auto shadow p-3 rounded-4 my-3">
    <div class="">
        <h1>My name is: {name}</h1>
        <h2>My name is: {age}</h2>
        <h3>my location is: {location}</h3>
        <h4>my hubby is: {hubby} </h4>
        <p>{@html simpleHTML}</p>
    </div>

            <!--#each-->
    <div>
        <!-- <h1>My friends are: {friends.join(", ")}</h1> -->
        <ul>
            {#each friends as friend}
                <li>{friend}</li>
            {/each}
        </ul>
    </div>
    <div>
        <h1>My favorite movies are:</h1>
        <ul>
            {#each movies as movie}
                <li>{movie.title} ({movie.year}) - {movie.genre}</li>
            {/each}
        </ul>
    </div>
    <div>
        {#if isVissible}
            <h4>The message is visible</h4>
        {/if}

        <button onclick={() =>isVissible = !isVissible}>toggle visibility</button>
    </div>
    <div>
        {#if score > 80}
        <p>Excellent</p>
        {:else if score > 70}
        <p>Good</p>
        {:else if score > 60}
        <p>Okay</p>
        {:else if score > 50}
        <p>Bad</p>
        {/if}
        <p>{score}</p>
        <button onclick={()=> score += 5}>increase score</button>
        <button onclick={()=> score -= 5}>decrease score</button>
    </div>
    <div>
        {#if hour < 12}
        <p>Good morning</p>
        {:else if hour < 18}
        <p>Good afternoon</p>
        {:else}
        <p>Good evening</p>
        {/if}
        <p>{hour}</p>
        <button onclick={()=> hour += 2}>Increase Hour</button>
        <button onclick={()=> hour -= 2}>Decrease Hour</button>
    </div>
    hou
    <div>
        <h1>My friends are:</h1>
        <ul>
            {#each friends as friend}
                <li>{friend}</li>
            {/each}
        </ul>
        <h1>My friends are:</h1>
        <ul>
    </div>
</header>