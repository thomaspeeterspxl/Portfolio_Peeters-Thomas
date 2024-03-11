<template>
  <nav id="navbar">
    <a href="index.html"><img src="@/assets/images/logo_nav.png" alt="nav_logo"></a>
    <ul>
      <li><a class="navbar-link" href="#">Home</a></li>
      <li><router-link class="navbar-link" to="/">Over mij</router-link></li>
      <li class="dropdown">
        <a  class="navbar-link" href="#">Projecten</a>
        <ul class="dropdown-menu">
          <li ><a href="/Project" class="dropdown-menu-item">Design</a></li>
          <li><a href="/Code" class="dropdown-menu-item">Code</a></li>
          <li><a href="/3d" class="dropdown-menu-item">3d</a></li>
          <li><a href="/animation" class="dropdown-menu-item">Animation</a></li>
        </ul>
      </li>
      <li class="dropdown">
        <a class="navbar-link" href="#">WPL</a>
        <ul class="dropdown-menu">
          <li><a href="/WPL1" class="dropdown-menu-item">wpl1</a></li>
          <li><a href="/WPL2" class="dropdown-menu-item">wpl2</a></li>
        </ul>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  mounted() {
    window.addEventListener('scroll', this.handleScroll);
  },
  methods: {
    handleScroll() {
      const navbar = document.getElementById('navbar');
      if (window.scrollY > 0) {
        navbar.classList.add('navbar-hidden');
      } else {
        navbar.classList.remove('navbar-hidden');
      }
    }
  }
}
</script>

<style scoped>

</style>
