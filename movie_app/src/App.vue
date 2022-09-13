<template>
  <header>
    <router-link to="/">
      <h1>Movies</h1>
    </router-link>
  </header>
  <main>
    <router-view></router-view> 
  </main>
  <router-view/>
</template>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Fira Sans', sans-serif;
  &::selection{
    background: transparentize($color: #42B883, $amount: 0.5)
  }
  body {
    background:  #778fa8;
  }
  a {
    text-decoration: none;
  }
  header{
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 10px 16px;
    background: #545b61;
    box-shadow: 0px 0px 6px rgba(0, 0, 0, 0.1);
  }
  h1{
    color: #fff;
    font-size: 28px;
    span{
      color: #42B883;
    }
  }
}
</style>
