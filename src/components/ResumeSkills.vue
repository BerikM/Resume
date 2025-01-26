<script lang="ts" setup>

const skills = [
  {
    name: "HTML",
    discription: 'HTML4/HTML5'
  },
  {
    name: "CSS3",
    discription: 'SASS/LESS5'
  },
  {
    name: "JS",
    discription: 'React JS'
  },
  {
    name: "JS",
    discription: 'Angular JS'
  },
]

</script>

<template>
  <section class="container">
    <article class="main">
      <h2 class="main__title">Programming skills</h2>
      <p class="main__more">Front end engineer believing in the power of web development. Experienced in all stages of advanced front end development.
         Focused on single-page application development, CSS/JS animations, semantics, accessibility, and progressive enhancement. However, I'm keen on
          exploring new languages and I always try to stay up-to-minute. Apart from these, I have other computer skills, such as I fluently use Adobe XD
          and Sketch for designing the websites before coding them. I also have basic knowledge in 3D Max Studio and Adobe After Effect and I use them as a hobby.
        </p>
    </article>

    <article class="skills">
      <div class="skill" v-for="skill in skills" :key="skill.name">
        <h2 class="skill__name">{{ skill.name }}</h2>
        <p class="skill_discription">{{ skill.discription }}</p>
      </div>
    </article>
  </section>
</template>

<style scoped>
.container{
  max-width: 1200px;
  margin: 0 auto;
  display: flex;
  align-items: center;
  padding: 80px 0px;
}

.main{
  padding: 0px 20px;
}

.main__title{
  font-size: 40px;
  margin-top: 0px;
}

.skills{
  display: grid;
  grid-auto-flow: column;
  grid-template-rows: 1fr 1fr;
  padding: 0px 20px;
}

.skill{
  height: 120px;
  padding: 0 14px;
  text-align: center;
}

.skill__name{
  font-weight: 700px;
  color: rgb(73, 175, 115);
  font-size: 50px;
  margin: 10px 0px;
}

.skill_discription{
  font-size: 18px;
  font-weight: 600;
}

</style>
