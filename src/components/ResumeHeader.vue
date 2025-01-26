<script lang="ts" setup>
import { ref } from 'vue';


const scrollTo = (sectionId:string)=> {
      const section = document.getElementById(sectionId);
      if (section) {
        section.scrollIntoView({ behavior: 'smooth' });
      }
    }

const isTop = ref(false);

window.addEventListener('scroll', () => {
  if(window.scrollY == 0){
    isTop.value = true;

  }else{
    isTop.value = false;
  }
});

</script>

<template>
  <header class="header" :class="{'hide':isTop}">
    <div class="header_container">
      <nav class="header_links">
        <a @click="scrollTo('about')" class="header_link">About</a>
        <a @click="scrollTo('skills')" class="header_link">Skills</a>
        <a @click="scrollTo('experience')" class="header_link">Experience</a>
        <a @click="scrollTo('portfolio')" class="header_link">Portfolio</a>
        <a @click="scrollTo('about')" class="header_link">Contact</a>
      </nav>
    </div>
  </header>
</template>

<style scoped>
header{
  background-color: black;
  height: 60px;
  width: 100%;
  position:fixed;
}
.header_container{
  max-width: 1200px;
  height: 100%;
  margin: 0px auto;
}
.header_links{
  display: flex;
  justify-content: flex-end;
  align-items: center;
  height: 100%;
}
.header_link{
  text-decoration: none;
  color: white;
  padding: 15px;
}

.header_link:hover{
  cursor: pointer;
}

.hide{
  background:none;
}
</style>
