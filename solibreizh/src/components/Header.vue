<script setup lang="ts">

</script>

<template>
  <div class="greetings">
    <img
      alt="logo"
      class="logo"
      src="@/assets/SoliBreizh.png"
      width="125"
      height="125"
    />
    <h1 class="green">Soli'Breizh</h1>
    <h3>
      Soli'Breizh
    </h3>
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

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
