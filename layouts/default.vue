<template>
  <div>
    <transition name="slide-fde">
      <MobileMenu v-show="showMobileMenu" @closeMobileMenu="showMobileMenu = false" />
    </transition>
    <MainHeader @showMobileMenu="showMobileMenu = true"/>
    <div class="h-screen flex">
      <Nuxt />
    </div>
  </div>
</template>

<style lang="scss">

p, h1, h2, h3, h4, h5, a {
  font-family: 'Kumbh Sans', sans-serif;
}

.slide-fade-enter-active {
  transition: all .3s ease;
}
.slide-fade-leave-active {
  transition: all .3s cubic-bezier(1.0, 0.5, 0.8, 1.0);
}
.slide-fade-enter, .slide-fade-leave-to
  {
  opacity: 0;
}
</style>

<script>
export default {
  data () {
    return {
      showMobileMenu: false
    }
  },
  watch: {
    '$route' () {
      this.showMobileMenu = false
    }
  },
}
</script>
