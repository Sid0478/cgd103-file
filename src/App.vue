<template>
  <header>
<header></header>
  </header>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
    <router-link to="/news">news</router-link>
    <router-link to="/product">product</router-link>
  </nav>
<p>哈哈哈</p>
  <router-view/>
  <images link="https://fakeimg.pl/300x200/200"/>
  <footer>footer</footer>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import images from '@/components/images.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld,
    images,
  }
}

</script>



<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

header{
  background-color:greenyellow;
  height: 10rem;
}

main{

}

footer{
background: gray;
height: 8rem;
}


nav {
  padding: 30px;;

  a {
    font-weight: bold;
    color: #2c3e50;
    margin: 2rem;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
