<template>
    <div class="main__container-header">
         <div class="container__nav">
          <div class="name-item">
            Dawood.dev
          </div>
          <div>
            <dev class="list">
              <dev><a class="list-item" href="#home">Home</a></dev>
              <dev><a class="list-item" href="#about">About</a></dev>
              <dev><a class="list-item" href="#projects">Projects</a></dev>
              <dev><a class="list-item" href="#contact">Contact</a></dev>
            </dev>
          </div>
        </div>
     </div>
  </template>
  
  <script setup>
  //
  </script>
  <style>
  .container__nav {
    box-shadow: rgba(0, 0, 0, 0.15) 1.95px 1.95px 2.6px;
    align-items: center;
    background-color: #fff;
    display: flex;
    font-size: 1.7rem;
    height: auto;
    justify-content: space-between;
     padding: 15px 40px 15px 50px;
      /* width: 100%; */
      position: fixed;
      width: 100%;
   }
  
  .list {
    flex-direction: row;
    display: flex;
    gap: 20px;
  }
  
  .list-item {
    font-size: 20px;
  
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
    z-index: 1;
  }
  </style>
  