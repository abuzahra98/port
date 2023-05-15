<template>
  <div class="main__container-header">
    <div class="container__nav">
      <div class="name-item">
        Dawood.dev
      </div>
      <div>
        <dev class="list" :class="['navbar-menu', { 'show': state.isMenuOpen }]">
          <dev><a class="list-item"  @click="toggleMenu" href="#home">Home</a></dev>
          <dev><a class="list-item"  @click="toggleMenu" href="#about">About</a></dev>
          <dev><a class="list-item"  @click="toggleMenu" href="#projects">Projects</a></dev>
          <dev><a class="list-item"  @click="toggleMenu" href="#contact">Contact</a></dev>

        </dev>

        

        <div  class="navbar-toggle" @click="toggleMenu">
          <img style="width: 35px;" src="/menu.png" alt="">
        </div>

      </div>
    </div>
  </div>
</template>
  
<script setup>
import { reactive } from 'vue';

const state = reactive({
  isMenuOpen: false
})

const toggleMenu = () => {
  state.isMenuOpen = !state.isMenuOpen;
}
</script>
<style>
.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 10px;
  background-color: #f0f0f0;
}

.navbar-logo {
  font-weight: bold;
}

.navbar-toggle {
  display: none;
   cursor: pointer;
}

.navbar-toggle .line {
  width: 25px;
  height: 3px;
  background-color: #888888;
  margin: 5px;
  transition: all 0.3s ease;
}

.navbar-menu {
  z-index: 333;

  display: flex;
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.navbar-menu li {
  margin: 0 10px;
}

 @media (max-width: 768px) {

  .navbar-toggle {
    display: block;
   }

  .navbar-menu {
    display: none;
   }

  .navbar-menu.show {
  
    display: flex;
    flex-direction: column;
    text-align: center;
    position: absolute;
    top: 100%;
    left: 0;
    width: 100%;
    background-color: #f0f0f0;
    padding: 10px;
  }

  .navbar-menu.show li {
    margin: 10px 0;
  }
}
 
.container__nav {
  box-shadow: rgba(0, 0, 0, 0.15) 1.95px 1.95px 2.6px;
  align-items: center;
  background-color: #fff;
  display: flex;
  font-size: 1.7rem;
  height: auto;
  justify-content: space-between;
  padding: 20px 60px 20px 50px;
  position: fixed;
  width: 100%;
}

.list {
  flex-direction: row;
  display: flex;
  gap: 20px;
}

.list-item {
  font-size: 18px;

  color: #2d2e32;
  font-weight: 600;
  text-decoration: none;
  transition: all 0.23s;
  text-decoration: none;
}

.list-item:hover {
  color: #147efb;
}

.name-item {
  display: block;
  font-size: 24px;
  margin: 0;
  font-weight: 900;
}

.main__container-header {
  z-index: 10;
}

@media (max-width: 768px) {
  .list {
    display: none;
  }
}
</style>
  