<script lang="ts" setup>

const languages:{name:string, level: string}[] = [
  {
    name: "English",
    level: "Native"
  },
  {
    name: "Russian",
    level: "Native"
  }
]

</script>

<template>
  <section class="languages">
    <div class="container">
      <h2 class="languages__title">Languages</h2>
      <div class="languages__list">
        <article v-for="lang in languages" :key = "lang.name" class="language">
          <h3 class="language__name">{{ lang.name }}</h3>
          <p class="language__level">{{ lang.level }}</p>
        </article>
      </div>
    </div>
  </section>
</template>

<style scoped>
  .languages{
    background-image: url("../assets/lang_bg.jpg");
    background-position: center;
    padding: 70px 0px;
  }

  .container{
    max-width: 1200px;
    height: auto;
    margin: 0px auto;
  }

  .languages__title{
    color: white;
    text-align: center;
    font-size: 3vw;
    margin-top: 20px;
    margin-bottom: 0px;
  }

  .languages__list{
    display: flex;
    justify-content: space-evenly;
  }

  .language{
    padding: 20px;
    text-align: center;
  }

  .language__name{
    color: rgb(73, 175, 115);
  }

  .language__level{
    color: white;
  }

</style>
