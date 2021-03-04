<script>
  //import { Router, Link, Route } from "svelte-routing";
  import { Route } from "svelte-micro";
  import Home from "./Home.svelte";
  import About from "./About.svelte";
  import Blog from "./Blog.svelte";

</script>


<Route>
  <!-- Always will be shown -->
  <nav>
    <a href="/">Home</a>
    <a href="/hello">About</a>
    <a href="/blog">Blog</a>
  </nav>

  <!-- Will be shown only when the page path is equal to the '/' -->
  <Route path="/">
    <h1>Home page</h1>
    <p>Feel at home!</p>
  </Route>
   <Route path="/hello">
    <h1>about page</h1>
    <p>Feel at home!</p>
  </Route>
  <Route path="/blog">
    <h1>Blog page</h1>
    <p>Feel at home!</p>
  </Route>
</Route>