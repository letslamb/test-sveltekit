<script>
	import '../app.css';
</script>

<nav>
  <div>
    <a href="/">Home</a>
    <a href="/about">About</a>
  </div>
</nav>
<slot />

<style>
  nav {
    display: flex;
  }

  div {
    margin: 0 auto;
  }
</style>
