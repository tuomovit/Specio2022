<template>
  <div class="header">
    <div class="container">
    <div class="wrapper">  
      <NuxtLink to="/">
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
      </NuxtLink>
      <div role="button" class="menu" @click="showMobileMenu">
        <div class="line"></div>
        <div class="line"></div>
        <div class="line short"></div>
      </div>
  </div>
  </div>
  </div>
</template>


<style lang="scss">
.header {
  padding-top: 3rem;
  padding-bottom: 2rem;
  height: 20vh;
  background-color: #3b664c;

  .wrapper {
    display: flex;
    justify-content: space-between;
  }
}

.menu {
  transition: all .3s ease;
.line {
  width: 40px;
  height: 2px;
  background: black;
  margin-top: 5px;
  pointer-events: all;
  &.short {
    width: 23px;
    transition: all .3s ease;
  }
}
&:hover {
  .short {
    width: 40px;
  }
} 
}

a:hover {
  text-decoration: none;
}

.dot {
  height: 15px;
  width: 15px;
  background-color: #dbdad8;
  border-radius: 50%;
  display: inline-block;
}
</style>

<script>
export default {
  methods: {
    showMobileMenu () {
      this.$emit('showMobileMenu')
    }
  }
}
</script>
