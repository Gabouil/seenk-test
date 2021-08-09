<template>
  <main>
    <Profil />
    <div class="main_container">
      <Personality />
      <Education />
      <WorkLife />
      <Hobbies />
      <DigitalCommunities />
      <DigitalMedia />
      <Goals />
      <Frustrations />
    </div>
  </main>
</template>

<script>
import Profil from '../components/Greg/Profil.vue'
import Personality from '../components/Greg/Personality.vue'
import Education from '../components/Greg/Education.vue'
import WorkLife from '../components/Greg/WorkLife.vue'
import Hobbies from '../components/Greg/Hobbies.vue'
import DigitalCommunities from '../components/Greg/DigitalCommunities.vue'
import DigitalMedia from '../components/Greg/DigitalMedia.vue'
import Goals from '../components/Greg/Goals.vue'
import Frustrations from '../components/Greg/Frustrations.vue'

export default {
  name: 'mainPage',
  components: {
    Profil,
    Personality,
    Education,
    WorkLife,
    Hobbies,
    DigitalCommunities,
    DigitalMedia,
    Goals,
    Frustrations
  }
}
</script>
<style>
main {
  background-color: #F4F4F4;
  display: grid;
  grid-template-columns: .35fr 1fr;
  grid-template-areas: 
    "Profil Container";
  height: 100vh;

}
.main_container {
  grid-area: Container;
  display: grid;
  grid-template-rows: .6fr 1fr .8fr .6fr;
  grid-template-columns: 1fr 1fr;
  grid-template-areas: 
    "Personality DigitalCommunities"
    "Education DigitalMedia"
    "WorkLife Goals"
    "Hobbies Frustrations";
  height: 100%;
  padding: 2%;
}

/* gestion des sections en général */
.main_section {
  padding: 5%;
}
.main_section h1 {
  margin-bottom: 15px;
  color: #626262;
}
.main_section {
  background-color: white;
  margin: 3%;
  box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.05);
  border-radius: 4px;
}
#Profil {
  grid-area: Profil;
}
#Personality {
  grid-area: Personality;
}
#Education {
  grid-area: Education;
}
#WorkLife {
  grid-area: WorkLife;
}
#Hobbies {
  grid-area: Hobbies;
}
#DigitalCommunities {
  grid-area: DigitalCommunities;
}
#DigitalMedia {
  grid-area: DigitalMedia;
}
#Goals {
  grid-area: Goals;
}
#Frustrations {
  grid-area: Frustrations;
}


/* responsive */
@media screen and (max-width: 1000px) {
  main {
    grid-template-columns: 1fr;
    grid-template-rows: 1fr 1fr;
    grid-template-areas: 
      "Profil"
      "Container";
    height: 100%;

  }
}
@media screen and (max-width: 600px) {
  main {
    grid-template-columns: 1fr;
    grid-template-rows: .5fr 1fr;
    grid-template-areas: 
      "Profil"
      "Container";
    height: 100%;

  }
  
  .main_container {
    grid-template-rows: .6fr 1fr .8fr .6fr .6fr 1fr .8fr .6fr;
    grid-template-columns: 1fr;
    grid-template-areas: 
      "Personality "
      "Education "
      "WorkLife "
      "Hobbies "
      "DigitalCommunities"
      "DigitalMedia"
      "Goals"
      "Frustrations";
    height: 100%;
    padding: 2%;
  }
}

</style>
