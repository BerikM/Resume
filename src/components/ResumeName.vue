<script lang="ts" setup>
</script>

<template>
  <div class="block_name">
    <div class="container">
      <div class="name_texts">
        <p class="name">Берик Мукин</p>
        <p class="spec">Front-End Developer</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.block_name{
  width: 100%;
  height: 460px;
  background-image: url('../assets//bg.webp');
  background-size: cover;
  background-position: center;
}

.container{
  max-width: 1024px;
  height: 100%;
  margin: 0 auto;
}

.name_texts{
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: 100%;
  align-items: center;

}

.name{
  font-size: 7vw;
  font-weight: 700;
  color: white;
  margin: 0;
  margin-top: 10vh;
}

.spec{
  font-size: 3vw;
  font-weight: 400;
  color: rgb(109, 219, 154);
  margin: 0;
  margin-top: 15vh;

}
</style>
