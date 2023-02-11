<script setup lang="ts">
</script>

<template>
    <section class="sectionCrew">
      <h2>Notre équipage</h2>
      <p>
        Notre équipage est composé des 3 membres de l'association Soli'Breizh :
      </p>
      <div class="crew1 crew">
        <div>
          <h3>Nolann MORENCé - 22 ans</h3>
          <span>Président de l’association Soli’Breizh. Originaire de Lorient (Morbihan)</span>
          <p>
            J’ai eu la chance de toujours avoir ce dont j’avais besoin
            durant ma vie, lorsque j’ai appris l’existence de cet
            événement, j’ai vu en lui une occasion en or d’aider des
            jeunes dans le besoin mais également de pouvoir vivre une
            aventure inoubliable à travers l’Europe avec deux super
            amis à bord d’une super voiture préparée par nos soins.
            Ce raid est l'occasion pour moi de révéler mon côté aventurier en pilotant la mythique Peugeot 205, 
            aujourd'hui considéré comme une voiture de collection, à travers l'Europe. 
            L'idée d'apporter mon aide à des écoliers en déposant des fournitures humanitaires dans une école en Europe de l'Est me plaît également. 
            Cette aventure risque d'être forte en émotion, je suis impatient de prendre le départ.
          </p>
        </div>
        <img src="@/assets/nolann.jpg" height="300"/>

      </div>
      <div class="crew2 crew">
        <img src="@/assets/lucas.jpg" height="300"/>
        <div>
          <h3>Lucas NICOD - 22 ans</h3>
          <span>Secrétaire de l’association Soli’breizh. Originaire de Concarneau (Finistère)</span>
          <p>
            Passioné d’automobile, j’ai tout de suite accroché à l’idée
de pouvoir faire l’Europ’Raid un jour. Toujours prêt à relever un défi, cette aventure va être l'occasion pour moi de découvrir de nouveaux pays, 
            des paysages encore jamais vus, tout cela avec 2 super amis, au volant d'une 205 et dans un but humanitaire ! Si c'est pas magique comme aventure ça...
            Je me vois déjà sillonner les routes d'Europe en vous partageant notre périple !
          </p>
        </div>
      </div>
      <div class="crew3 crew">
        <div>
          <h3>Clément LEPROVOST - 23 ans</h3>
          <span>Trésorier de l’association Soli’Breizh. Originaire de Lannion (Côtes-d’Armor)</span>
          <p>
            Cette aventure promet d'être riche en surprises et en émotions. 
            J'ai hâte de pouvoir contribuer à ce projet solidaire via ce voyage en 205 qui s'annonce inoubliable.
             C'est un message engagé à faire passer aux générations futures que l'on va découvrir. 
             Je suis pressé de vivre ce voyage avec mes amis et de faire partager le goût de l'aventure avec tous les gens qui vont nous soutenir lors de ce projet.
             Prêt à relever tous les défis, j’ai tout de suite accepté la
              proposition de me lancer dans cette aventure avec mes deux amis. Je suis paré à faire ce voyage incroyable autour de l’Europe.
          </p>
        </div>
        <img src="@/assets/clement.jpg" height="300"/>
      </div>
    </section>
</template>

<style>
.sectionCrew{
  background-color: #0A72CC;
  color: white;
  padding-bottom: 10px;
}

.sectionCrew h2 {
  padding: 10px 30px;
  text-decoration: underline;
}

.sectionCrew p {
  padding-left: 30px;
}

.crew1 {
  background-color: #00BFB2;
}

.crew2 {
  background-color: #08A36D;
}

.crew3 {
  background-color: #09B046;
}

.crew{
  display: flex;
  width: 95vw;
  justify-content: space-between;
  margin: 10px 20px;
  padding: 10px;
  border-radius: 5px;
}

.crew img{
  border-radius: 10px;
}

.crew div
{
  margin: 10px;
}

h3{
  text-decoration: underline;
}
</style>
