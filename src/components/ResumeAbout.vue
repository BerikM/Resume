<script lang="ts" setup>
</script>

<template>
  <div class="about">
    <div class="container">
      <div class="about_text size">
        <p class="text_title green">I code, therefore I am.</p>
        <p class="text_text">I am a young enthusiast who is keen on IT and anything about it since my first steps to High School.
          During the past few years, I gained lots of experience in this field due to the strong desire of b
          ecoming an expert. Today I am a senior front-end developer at one of the leading companies in the world. </p>
      </div>
      <div class="about_me size">
        <h3 class="city">Проживание: Казахстан, Павлодар</h3>
        <p class="years green">22 года</p>
        <img src="../assets/face.jpeg" alt="" srcset="" class="face">
      </div>
    </div>
  </div>
</template>

<style scoped>
.about{
  padding: 80px 0px;
}

.container{
  max-width: 1024px;
  height: auto;
  margin: 0px auto;
  display: flex;
  justify-content: space-between;
}

.size{
  width: 40%;
}

.face{
  width: 300px;
  height: 300px;
  object-fit: cover;
  object-position: center;
  border-radius: 50%;
}

.text_title{
  font-size: 4vw;
}

.green{
  color: rgb(109, 219, 154);
}

.text_text{
  color: rgb(66, 84, 117);
}

.about_me{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

</style>
