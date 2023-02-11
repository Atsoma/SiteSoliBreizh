<script setup lang="ts">
  function reveal()
  {
    var reveals = document.querySelectorAll(".reveal");
    for (var i = 0; i < reveals.length; i++) {
      var windowHeight = window.innerHeight;
      var elementTop = reveals[i].getBoundingClientRect().top;
      var elementVisible = 150;
      if (elementTop < windowHeight - elementVisible) {
        reveals[i].classList.add("active");
      } else {
        reveals[i].classList.remove("active");
      }
    }
  }

  window.addEventListener("scroll", reveal);

  reveal();

</script>

<template>
  <main>
    <div class="sectionCustom">
      <h3>Soli'Breizh X Europ'Raid</h3>
      <p>
        Du 29 juillet au 19 août 2023 aura lieu l'EuropRaid, un raid humanitaire en Europe dans lequel chaque équipage voyage en Peugeot 205. 
        Lors de cet événement, nous devons avoir au départ 70 kg de fourniture humanitaire à bord de la voiture, le tout sera distribué à une population dans le besoin. 
        Pour mieux vous représenter l'événement, voici les chiffres clés :
      </p>
      <div class="listKey">
        <div class="KeyNum">
          <u><span class="kmNum reveal"></span> km</u>
          <div>à parcourir</div>
        </div>
        <div class="KeyNum">
          <u><span class="kgNum reveal"></span> kg</u>
          <div>de matériel Solidaire</div>
        </div>
        <div class="KeyNum">
          <u><span class="paysNum reveal"></span> pays</u>
          <div>à travers l'Europe</div>
        </div>
        <div class="KeyNum">
          <u><span class="dayNum reveal"></span> jours</u>
          <div>de voyage</div>
        </div>
      </div>
    </div>
    <img src="@/assets/cover.jpg" style="width: 100%; height: auto; margin-bottom: -10px;"/>
    <div class="sectionCustom flexSection" style="background-color: #09B046;">
      <p>
        Lors de ce raid, nous ferons escale dans 23 villes partenaires de
        l’événement et dans certaines écoles d’Europe de l’Est. Cette aventure nous
        permet également de partir à la découverte de l’Europe, de sa culture et de ses
        paysages magnifiques. L’itinéraire relie plus de 200 étapes, 13 capitales et
        environ 100 patrimoines de l’Unesco, le tout relié par les plus belles routes
        d’Europe. Chaque soir, les équipages sont réunis dans un bivouac à l’intérieur d’un
        lieu inédit où sont organisées des soirées culturelles.
      </p>
      <img src="@/assets/itineraire-2022.png" class="itin"/>
    </div>
    <div class="sectionCustom">
      <p>
        Nous participons à cet événement au nom de notre association, Soli’Breizh.
        Cette association a pour but de permettre à ses membres de participer à des
        événements solidaires/humanitaires, chaque membre résidant en Bretagne.
      </p>
    </div>
  </main>
</template>

<style>

.listKey{
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
  margin: 1em 3em;
}

.KeyNum{
  width: 30vw;
  text-align: center;
  margin: 1em;
  background-color: #09B046;
  border-radius: 25px;
  padding: 0.5em 0em;

}

.KeyNum a:hover, .KeyNum a:active, .KeyNum a:link, .KeyNum a:visited{
  color: white;
}

.sectionCustom{
  background-color: #08A36D;
  color: white;
  padding: 2em;

}

.itin{
  width: 35vw;

}

.flexSection{
  display: flex;
}

@property --numKm {
  syntax: "<integer>";
  initial-value: 0;
  inherits: false;
}

@property --numKg {
  syntax: "<integer>";
  initial-value: 0;
  inherits: false;
}

@property --numPay {
  syntax: "<integer>";
  initial-value: 0;
  inherits: false;
}

@property --numDay {
  syntax: "<integer>";
  initial-value: 0;
  inherits: false;
}

.kmNum.reveal {
  counter-increment: num var(--numKm);
  font: 800 40px system-ui;
}

.kmNum.reveal.active {
  animation: counterKm 3s ease-in-out 1 forwards;
}

.kmNum::after {
  content: counter(num);
}

.kgNum.reveal {
  counter-increment: num var(--numKg);
  font: 800 40px system-ui;
}

.kgNum.reveal.active {
  animation: counterKg 4s ease-in-out 1 forwards;
}

.kgNum::after {
  content: counter(num);
}

.paysNum.reveal {
  counter-increment: num var(--numPay);
  font: 800 40px system-ui;
}

.paysNum.reveal.active {
  animation: counterPay 1s ease-in-out 1 forwards;
}

.paysNum::after {
  content: counter(num);
}

.dayNum.reveal {
  counter-increment: num var(--numDay);
  font: 800 40px system-ui;
}

.dayNum.reveal.active {
  animation: counterDay 1s ease-in-out 1 forwards;
}

.dayNum::after {
  content: counter(num);
}

@keyframes counterKm {
  from {
    --numKm: 0;
  }
  to {
    --numKm: 8000;
  }
}

@keyframes counterKg {
  from {
    --numKg: 0;
  }
  to {
    --numKg: 19600;
  }
}

@keyframes counterPay {
  from {
    --numPay: 0;
  }
  to {
    --numPay: 20;
  }
}
@keyframes counterDay {
  from {
    --numDay: 0;
  }
  to {
    --numDay: 22;
  }
}

@media (max-width: 525px) {
  .KeyNum{
    width: 45vw;
  }
}

@media (max-width: 800px) {
  .flexSection{
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
  }

  .itin{
    width: 60vw;
  }
}


</style>
