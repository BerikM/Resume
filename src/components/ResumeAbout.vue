<script lang="ts" setup>
</script>

<template>
  <section class="about">
    <div class="mx-auto my-0 flex justify-between max-w-300">
      <article class="about_text size">
        <p class="text_title green">I code, therefore I am.</p>
        <p class="text_text">I am a young enthusiast who is keen on IT and anything about it since my first steps to High School.
          During the past few years, I gained lots of experience in this field due to the strong desire of b
          ecoming an expert. Today I am a senior front-end developer at one of the leading companies in the world. </p>
      </article>
      <article class="about_me size">
        <h3 class="city">Проживание: Казахстан, Павлодар</h3>
        <p class="years green">22 года</p>
        <img src="../assets/face.jpeg" class="face">
      </article>
    </div>
  </section>
</template>

<style scoped>
.about{
  padding: 80px 0px;
}

.size{
  width: 40%;
}

.face{
  max-width: 100%;
  object-fit: cover;
  aspect-ratio: 1;
  border-radius: 50%;
}

.text_title{
  font-size: 4vw;
  font-weight: 600;
  margin-top: 0px;
}

.green{
  color: rgb(73, 175, 115);
}

.text_text{
  color: rgb(66, 84, 117);
  line-height: 1.5;
}

.about_me, .about_text{
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin: 0px 20px;
}

.about_me{
  align-items: center;
}

.city{
  margin: 0;
}

</style>
