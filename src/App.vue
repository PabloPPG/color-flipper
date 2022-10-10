<template>
  <div id="header-background">
    <div id="header" class="container">
      <a href="/" id="logo">
        <img
          src="@/assets/color-circle.png"
          alt="A color wheel gradient"
          width="50"
          height="50"
        />
        <p>Color Flipper!</p>
      </a>
      <nav>
        <router-link class="router" to="/simple">Simple</router-link>
        <router-link class="router" to="/hex">Hex</router-link>
      </nav>
    </div>
  </div>
  <router-view />
</template>

<style>
html,
body {
  margin: 0;
  padding: 0;
}
.router {
  margin-left: 3rem;
}
.container {
  margin: auto;
  width: 85%;
}
#header-background {
  background-color: #b7f7c2;
}
#header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0.5rem 2rem;
  font-size: 1.5rem;
}
#header a {
  text-decoration: none;
  color: black;
}
#header a > p {
  margin-left: 1.5rem;
}
#logo {
  display: flex;
  align-items: center;
}
</style>
