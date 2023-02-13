<script lang="ts">

export default {
  name: "App",
  data() {
    return {
      screenWidth: 0,
    };
  },
  mounted() {
    this.updateScreenWidth();
    this.onScreenResize();
  },
  methods: {
    onScreenResize() {
      window.addEventListener("resize", () => {
        this.updateScreenWidth();
      });
    },
    updateScreenWidth() {
      this.screenWidth = window.innerWidth;
    },
  },
};

const test = false;

</script>

<template>
  <div class="wrapper">
    <div class="greetings">
      <img
        alt="logo"
        class="logo"
        src="@/assets/SoliBreizh.png"
      />
      <h1 style="color: white; font-weight: bold;">Soli'Breizh</h1>
      <h3 style="color: white; font-weight: bold;">
        Rejoignez l'aventure Soli'Breizh
      </h3>
      
    </div>
    <nav>
      <RouterLink to="/">Accueil</RouterLink>
      <RouterLink to="/crew">Équipage</RouterLink>
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
  width: 20vh;
  height: 20vh;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

.wrapper
{
  display: flex;
  justify-content: center;
  height: 80vh;

}

nav {
  width: 100%;
  font-size: 18px;
  text-align: center;
  margin: 1rem;
}

nav a.router-link-exact-active {
  color: white;
}

nav a:visited, nav a:link
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

header{
  display: flex;
  place-items: center;
}

header .wrapper {
  display: flex;
  place-items: flex-start;
  flex-wrap: wrap;
}

@media (max-width: 920px) {
  header {
    display: flex;
    place-items: center;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
    height: 50vh;
  }  
}

</style>
