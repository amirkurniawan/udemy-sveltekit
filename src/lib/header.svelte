<script>
    export let title;
</script>

<header>
    <h1><a href="/" sveltekit:prefetch>{title}</a></h1>
    <nav>
      <a href="/posts" sveltekit:prefetch>POST</a>
      <a href="/about" sveltekit:prefetch>ABOUT</a>
      <a href="/login" sveltekit:prefetch>LOGIN</a>
    </nav>
</header>



<style lang="scss">
    header {
    background-color: aquamarine;
    padding: 15px;
    display: flex;

    h1 {
      flex: 1;
      margin: 0;

      a {
        color: purple;
        text-decoration: none;
      }
    }
  }

  nav{
    display: flex;
    align-items: center;
    a {
      color: sienna;
      border-right: 3px solid sienna;
      font-weight: bold;
      padding: 0 15px;
      text-decoration: none;
      transition: 0.2s;

      &:last-child{
        border-right: none;
      }
      &:hover{
        color: salmon;
      }
    }
  }
</style>