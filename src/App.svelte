<script>
  import "./app.css";
  import Router from "svelte-spa-router";
  import { link } from "svelte-spa-router";
  import Quiz from "./routes/Quiz.svelte";
  import Home from "./routes/Home.svelte";
  
  const routes = { "/": Home, "/quiz": Quiz };
</script>
<div class="bg-success">
  <a use:link href="/">Home</a>
  <a use:link href="/quiz">Quiz</a>
</div>
  

  <main class="">
  <Router {routes} />
</main>
