<template>
    <nav class="navbar">
      <div class="navbar-logo">Logo</div>
      <div class="navbar-toggle" @click="toggleMenu">
        <div class="line"></div>
        <div class="line"></div>
        <div class="line"></div>
      </div>
      <ul :class="['navbar-menu', { 'show': isMenuOpen }]">
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </template>
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
  display: none; /* Hide the toggle button on larger screens */
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
  display: flex;
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.navbar-menu li {
  margin: 0 10px;
}

/* Media Query for smaller screens */
@media (max-width: 768px) {
  .navbar-toggle {
    display: block; /* Show the toggle button on smaller screens */
  }

  .navbar-menu {
    display: none; /* Hide the menu items on smaller screens */
  }

  .navbar-menu.show {
    display: flex; /* Show the menu items when the toggle button is clicked */
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

</style>