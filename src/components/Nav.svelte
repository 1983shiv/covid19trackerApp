<script>
  export let segment;
  export let isOpen = false;

  function toggleNav() {
    isOpen = !isOpen;
  }
</script>

<nav class="navbar" role="navigation" aria-label="main navigation">
  <div class="navbar-brand">
    <a class="navbar-item" href="/">
      <img src="c19virus.png" alt="Covid19 Tracker App" />
    </a>

    <span
      href="/"
      role="button"
      class="navbar-burger"
      aria-label="menu"
      aria-expanded="false"
      data-target="navbarBasicExample"
      on:click={toggleNav}
      class:is-active={isOpen}
    >
      <span aria-hidden="true" />
      <span aria-hidden="true" />
      <span aria-hidden="true" />
    </span>
  </div>

  <div id="navbarBasicExample" class="navbar-menu" class:is-active={isOpen}>
    <div class="navbar-start">
      <a
        aria-current={segment === undefined ? "page" : undefined}
        href="/"
        class="navbar-item"
      >
        Home
      </a>
      <a
        aria-current={segment === "about" ? "page" : undefined}
        href="about"
        class="navbar-item"
      >
        About
      </a>
    </div>
  </div>
</nav>

<style>
  .navbar {
    border-bottom: solid 1px #cecece;
    margin-bottom: 20px;
  }
</style>
