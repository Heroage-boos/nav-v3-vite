<template>
  <nav class="nav">
    <!-- <router-link to="/">Home</router-link> 
    <router-link to="/about">About</router-link> -->
    <!-- <router-view to="/" /> -->
    <div class="logo">
      <a href="#"><img src="logo.png" alt="Logo"></a>
    </div>
    <div class="menu">
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">chat</a></li>
        <li><a href="#">壁纸</a></li>
        <li><a href="#">更多</a></li>
      </ul>
    </div>
  </nav>
  <div class="container">
    <router-view to="/" />
  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  display: flex;
  flex-direction: column;
  height: 100%;

  color: #2c3e50;
}

.nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px;
}
.container{
  flex: 1;
}

.logo img {
  height: 50px;
}

.menu {
  flex-direction: column;

  ul {
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0;
    padding: 0;
    list-style: none;
  }

}

.menu li {
  margin: 0 10px;
}

.menu a {
  text-decoration: none;
  color: #333;
  font-weight: bold;
}
</style>
