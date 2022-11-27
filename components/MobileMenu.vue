<template>
    <div>
      <div class="mobile-menu">
        <div class="container">
        <div class="menu-wrapper">
            <div class="links">
                <NuxtLink class="link" to="/vk2022">Vuosikokous 2022</NuxtLink>
                <NuxtLink class="link" to="/">Vuosikokous 2020</NuxtLink>
                <NuxtLink class="link" to="/">Vuosikokous 2019</NuxtLink>
            </div>
            <div class="button">
            <button @click="closeMobileMenu" class="remove">
                <span class="x eka"></span>
                <span class="x toka"></span>
            </button>
        </div>
            </div>
      </div>
    </div>
    </div>
  </template>
  
  <script>
  export default {
    methods: {
      closeMobileMenu () {
        this.$emit('closeMobileMenu')
      }
    }
  }
  </script>

<style lang="scss">

.link {
  opacity: 0;
  animation: fadeIn 1.2s 1;
  animation-fill-mode: forwards;
}

@keyframes fadeIn {
  0% {
    opacity: 0.0;
  }
  100% {
    opacity: 1.0;
  }
}


.mobile-menu {
  padding-top: 3rem;
  position: absolute;
  width: 100%;
  height: 100%;
  background-color: antiquewhite;
  z-index: 10;
}

.menu-wrapper {
  display: flex;
  justify-content: space-between;
}

.links {
    margin-top: 4rem;
    display: flex;
    flex-direction: column;

    .link {
        font-size: 2rem;
        margin-bottom: 1rem;
        color: rgb(94, 94, 94);
        font-weight: 700;
    }

}

.remove {
    height: 40px;
    width: 40px;
    padding-right: 30px;
    background-color: transparent;
    border: none;
    font-size: 3rem;
    .x {
        width: 40px;
        height: 2px;
        position: absolute;
        background-color: black;
        transition: all .3s ease;
        &.eka {
            transform: rotate(135deg);
        }
        &.toka {
            transform: rotate(-135deg);
        }
    }
}
</style>