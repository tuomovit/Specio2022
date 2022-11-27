<template>
  <div class="hero">
    <div class="container">
      <h1 class="hero-title">SPECIO<span class="r-item">®</span></h1>
    </div>
  </div>
  
</template>

<style lang="scss">
$container-max-widths: (
  sm: 540px,
  md: 720px,
  lg: 960px,
  xl: 1140px,
  xxl: 1320px
);

.hero {
  padding-top: 3rem;
  height: 80vh;
  background-color: #3b664c;
}

.hero-title {
  display: flex;
  font-size: 13.5vw;
  color: #b3af90;
  @media (min-width: 1200px) { 
    font-size: 220px;
   }

   .r-item {
    font-size: 10.5vw;
    @media (min-width: 1200px) { 
    font-size: 150px;
   }
   }
}

</style>

<script>
export default {
  name: 'NuxtTutorial'
}
</script>
