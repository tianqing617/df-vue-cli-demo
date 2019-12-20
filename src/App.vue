<template>
  <div id="app">
    <section class="header">
      头部
    </section>
    <section class="main">
      <div class="sidebar">
        <router-link to="/" class="nav-home">Home</router-link>
        <router-link to="/about">About</router-link>
      </div>
      <div class="content">
        <router-view/>
      </div>
    </section>
  </div>
</template>

<style scoped lang="scss">
#app {
  display: flex;
  flex-direction: column;
  height: 100vh;
}
.header {
  text-align: center;
  font-size: 20px;
  height: 150px;
  line-height: 100px;
  border: 1px solid #CCC;
}
.main {
  height: 100%;
  display: flex;
  flex-direction: row;
  border: 1px solid red;
}
.sidebar {
  width: 100px;
  border: 1px solid blue;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  .nav-home {
    margin-bottom: 120px;
  }
}
.content {
  margin-left: 20px;
}
</style>
