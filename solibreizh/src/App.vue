<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import Header from "./components/Header.vue";

</script>

<template>
  <header>
      <Header />
  </header>
  <RouterView />
  <footer style="background-color: #0A72CC; color: white; display: flex; justify-content: space-around; flex-wrap: wrap;">
    <div style="margin : 20px">
      <div class="itemFooter">
        <span style="display: flex; align-items: center;  margin-right: 10px;"><img src="@/assets/email.png" alt="mail" width="40">Notre Adresse Mail :</span>
        <a href="mailto:soli.breizh@hotmail.com">soli.breizh@hotmail.com</a>
      </div>
      <div class="itemFooter">
        <div class="itemFooter">
          <span style="display: flex; align-items: center; margin-right: 10px;"><img src="@/assets/phone.png" alt="phone" width="40">Nos Numéros de téléphone :</span>
        </div>
      
        <ul style="list-style-type:none; padding: 10px;">
          <li><a href="tel:+33670031329">Nolann : +33 6 70 03 13 29</a></li>
          <li><a href="tel:+33778832337">Lucas : +33 7 78 83 23 37</a></li>
          <li><a href="tel:+33781581481">Clément : +33 7 81 58 14 81</a></li>
        </ul>
      </div>
    </div>
    
    <div class="itemFooter" style="flex-direction: row;">
      <a href="https://www.facebook.com/profile.php?id=100088813694956"><img src="@/assets/Facebook.png" alt="facebook" width="50"></a>
      <a href="https://www.instagram.com/soli.breizh/"><img src="@/assets/instagram.webp" alt="instgram" width="50"></a>
      <a href="https://twitter.com/SoliBreizh"><img src="@/assets/twitter.png" alt="twitter" width="50"></a>
      <a href="https://www.linkedin.com/in/soli-breizh-24a340256/"><img src="@/assets/LinkedIn.png" alt="linkedin" width="50"></a>
    </div>
  </footer>
</template>

<style scoped>
  header{
    background-image: url(./assets/europraid-1.jpg);
    background-attachment: fixed;
  }

  body{
    font-family: Arial, Helvetica, sans-serif !important;
  }

  .itemFooter{
    display: flex;
    align-items: center;
  }

  .itemFooter img {
    margin-right: 20px;
  }

  @media (max-width: 800px) {
    footer {
      height: 50vh;
    }
  }

  a:link {
    color: white;
  }

</style>
