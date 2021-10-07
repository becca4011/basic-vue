<template>
  <div id="app">
    <div id="nav">
      <!-- a 태그 대신, router-link를 사용 / index.js에서 설정한 path로 to 안에 넣기 -->
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <!-- Home을 누르면 Home 컴포넌트, About을 누르면 About 컴포넌트로 바뀜 (f12로 관찰 가능) -->
    <router-view />
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
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
