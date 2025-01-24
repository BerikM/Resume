<script lang="ts" setup>
</script>

<template>
  <header class="header">
    <div class="header_container">
      <nav class="header_links">
        <a href="#" class="header_link">About</a>
        <a href="#" class="header_link">Skills</a>
        <a href="#" class="header_link">Experience</a>
        <a href="#" class="header_link">Portfolio</a>
        <a href="#" class="header_link">Contact</a>
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
  max-width: 1024px;
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
</style>
