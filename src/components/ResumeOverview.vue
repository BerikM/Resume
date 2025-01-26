<script lang="ts" setup>

const blocks = [
  {
    title: "Skills",
    description: "Learn about my skills in programming, find info on my language knowledge and more.",
    link: "skills",
    logo: "skills.png"
  },
  {
    title: "Experience",
    description: "Get to know the timeline of my education and find out more about my working experience.",
    link: "experience",
    logo: "star.png"
  },
  {
    title: "Portfolio",
    description: "My portfolio is my biggest pride. Check my previous works and get to know my skills better.",
    link: "portfolio",
    logo: "portfolio.png"
  }
];

const scrollTo = (sectionId:string)=> {
      const section = document.getElementById(sectionId);
      if (section) {
        section.scrollIntoView({ behavior: 'smooth' });
      }
    }

</script>

<template>
  <section class="overview">
    <div class="container">
      <article class="overview__block" v-for="block in blocks" :key="block.title">
        <div class="overview__circle">
          <img v-bind:src="block.logo" class="overview__logo">
        </div>
        <h2 class="overview__title">{{ block.title }}</h2>
        <p class="overview__discription">{{ block.description }}</p>
        <a @click="scrollTo(block.link)" class="overview__link">
          Learn more
          <svg width="32" height="32" viewBox="0 0 32 32" class="arrow"><path d="M11.438 21.813l6.125-6.125-6.125-6.125 1.875-1.875 8 8-8 8z"></path></svg>
        </a>
      </article>

    </div>
  </section>

</template>

<style scoped>

.overview{
  padding: 80px 0px;
  background-color: rgb(28, 28, 29);
}

.container{
  max-width: 1200px;
  height: auto;
  margin: 0px auto;
  display: flex;
  justify-content: space-between;
  color: white;
}

.overview__block{
  display: flex;
  flex-direction: column;
  margin: 0px 20px;
  text-align: center;
  align-items: center;
}

.overview__circle{
  width: 60px;
  height: 60px;
  background-color: rgb(109, 219, 154);
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.overview__title{
  margin-top: 20px;
  font-weight: 600;
}

.overview__discription{
  margin: 0px;
  line-height: 1.2;
}

.overview__link{
  color: rgb(109, 219, 154);
  text-decoration: none;
  display: flex;
  align-items: center;
  margin-top: 20px;
}

.overview__link:hover{
  color: rgb(74, 180, 119);
}

.arrow{
  stroke:  rgb(109, 219, 154);
  fill:  rgb(109, 219, 154);
  transition: transform 0.3s ease;
}

.overview__link:hover .arrow{
  transform: translateX(5px);
}

.overview__logo{
  width: 50%;
  height: auto;
}


</style>
