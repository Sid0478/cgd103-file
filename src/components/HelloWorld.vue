<template>
  <div class="hello" :class = "type">
    <div class="img" v-for="item in 9" :key="item">
      <button>搶票囉</button>
      <img :src="require('@/assets/images/green-food-1.jpg')">
    </div>
    
    <h1>{{ title }}</h1>
    <h1>{{ msg }}</h1>
 
   
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
    title:String,
    type:String,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.img{
  background-color: #42b983;
  width: 80vw;
  height: 6rem;
  margin: 3rem;
}

img{
  width: 100%;
}

.hello{
width: 10px;
display: flex;
}

h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
