<script lang="ts" setup>
interface Experience{
  years: string,
  name: string,
  spec: string
}
  const education: Experience[] = [
    {
      years: '2022-2025',
      name: 'Павлодарский государственный университет',
      spec: 'Computer Science - Frontend developer'
    },
    {
      years: '2018-2022',
      name: 'Павлодарский государственный колледж при университете',
      spec: 'Техник-программист'
    }
  ]

  const work: Experience[] = [
    {
      years: '2022-2025',
      name: 'Strong-Soft',
      spec: 'Создание frontend приложений на Typescript на базе библиотеки Pixi.js'
    }
  ]

</script>

<template>
    <section class="experience">
      <div class="container">
      <h2 class="experience__title">Experience</h2>

      <article class="experience__container">
        <img src="../assets/exp.webp" alt="image education" class="experience__image">
        <div class="education__list">
          <h3>Education</h3>
          <div class="history" v-for="(entry, index) in education" :key="index">
            <p>{{ entry.years }} <br>
            {{ entry.name }} <br>
            {{ entry.spec }}</p>
          </div>
        </div>
      </article>

      <article class="experience__container">
        <div class="education__list work">
          <h3>Work Experience</h3>
          <div class="history" v-for="(entry, index) in work" :key="index">
            <p>{{ entry.years }} <br>
            {{ entry.name }} <br>
            {{ entry.spec }}</p>
          </div>
        </div>
        <img src="../assets/exp.webp" alt="image work" class="experience__image">
      </article>

    </div>
    </section>
</template>

<style scoped>
  .experience{
    padding: 80px 0px;
  }

  .container{
    max-width: 1200px;
    margin: 0px auto;
  }

  .experience__title{
    text-align: center;
    font-weight: 600;
    font-size: 40px;
  }

  .experience__image{
    width: 40%;
    height: auto;
    padding: 0px 30px;
  }

  .experience__container{
    display: flex;
    justify-content: space-around;
    margin: 40px 20px;
    align-items: center;
  }

  .history{
    margin-top: 20px;
    color: rgb(66, 84, 117);
  }

  .work{
    text-align: right;
  }

  .education__list{
    width: 40%;
    padding: 0px 40px;
  }

</style>
