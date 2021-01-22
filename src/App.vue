<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>

      <div class="p-3 bg-green-500 text-white a">
        Hello Tailwind CSS
        <div class="p-3 bg-red-500 text-white b">Hello Tailwind CSS
          <div class="p-3 bg-blue-500 text-white c">Hello Tailwind CSS</div>
        </div>
      </div>
    </div>
    <router-view />
  </div>
</template>

<style lang="less" scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  .a{
    font-size: 30px;
    .b{
      font-size: 16px;
      .c{
        font-size: 20px;
      }
    }
  }
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
