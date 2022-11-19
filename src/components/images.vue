<template>
    <div class="img">
        <img :src="link" alt="">
    </div>
    <div class="img">
        <img :src="link" alt="">
    </div>
</template>

<script>
export default {
  // name: 'images',
  props: {
    link: String,
  }
}
</script>


<style lang="scss">

.img{
    width: 100vw;
    height: 18rem;
    background-color:rgb(167, 129, 102) ;
}

</style>
