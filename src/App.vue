<template>
  <div id="app">
    <div id="nav">
    </div>
    <router-view />
  </div>
</template>

<style lang="scss">
#app {
 width: 100%;
 height: 100;
 display: flex;
}

#nav {
  padding: 30px;

  span {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }

}
</style>
