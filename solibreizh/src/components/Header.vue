<script setup lang="ts">

</script>

<template>
  <div class="wrapper">
    <div class="greetings">
      <img
        alt="logo"
        class="logo"
        src="@/assets/SoliBreizh.png"
        width="125"
        height="125"
      />
      <h1 style="color: white; font-weight: bold;">Soli'Breizh</h1>
      <h3 style="color: white; font-weight: bold;">
        Rejoignez l'aventure Soli'Breizh
      </h3>
    </div>
    <nav>
      <RouterLink to="/">Accueil</RouterLink>
      <RouterLink to="/membres">équipage</RouterLink>
      <RouterLink to="/contact">Contact</RouterLink>
    </nav>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

.wrapper
{
  display: flex;
  justify-content: center;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: white;
}

nav a:visited
{
  color: white;
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid white;
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}

@media (min-width: 1024px) {
  
}
</style>
