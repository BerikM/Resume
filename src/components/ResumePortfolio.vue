<script lang="ts" setup>
import portfolioImage from '../assets/port_work.jpg';

const works = [
  {
    name: 'work 1',
    image: portfolioImage,
    discription: 'Описание',
    link: 'https://google.com'
  },
  {
    name: 'work 2',
    image: portfolioImage,
    discription: 'Описание',
    link: 'https://google.com'
  },
  {
    name: 'work 3',
    image: portfolioImage,
    discription: 'Описание',
    link: 'https://google.com'
  }
  ,
  {
    name: 'work 4',
    image: portfolioImage,
    discription: 'Описание',
    link: 'https://google.com'
  }
  ,
]

</script>

<template>
  <div class="portfolio">
    <h2 class="portfolio__title">Portfolio</h2>
    <div class="portfolio_works">
      <figure class="image-container" v-for="work in works" :key="work.name">
        <img :src="portfolioImage" alt="Изображение недоступно" >
        <figcaption>
          <p class="work_discription">{{ work.discription }}</p>
          <a class="work__link" :href="work.link">
            Посмотреть
            <svg width="32" height="32" viewBox="0 0 32 32" class="arrow"><path d="M11.438 21.813l6.125-6.125-6.125-6.125 1.875-1.875 8 8-8 8z"></path></svg>
          </a>
        </figcaption>
      </figure>
    </div>
  </div>
</template>

<style scoped>

.portfolio{
  padding: 40px 0px;
  text-align: center;
}

.portfolio__title{
  font-size: 3rem;
}

.portfolio_works{
  display: flex;
}

.image-container {
  position: relative;
  overflow: hidden;
  margin: 0px;
}

.image-container img {
  display: block;
  width: 100%;
  height: auto;
}

.image-container figcaption {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  background: rgba(0, 0, 0, 0.1);
  color: white;
  text-align: center;
  padding: 10px 0;
  transform: translateY(100%);
  transition: transform 0.3s ease;
}

.image-container:hover figcaption {
  transform: translateY(0);
}

.work_discription{
  margin-top: 0px;
  margin-bottom: 10px;
}

.work__link{
  text-decoration: none;
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
}

.work__link:hover{
  color: rgb(180, 178, 178);
}

.work__link:hover .arrow{
  transform: translateX(5px);
  fill:  rgb(180, 178, 178);
}

.arrow{
  fill: white;
  transition: transform 0.3s ease;
}



</style>
