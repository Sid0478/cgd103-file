<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
  <Space direction="vertical">
      <Space wrap>
          <Button>Default</Button>
          <Button type="primary">Primary</Button>
          <Button type="dashed">Dashed</Button>
          <Button type="text">Text</Button>
      </Space>
      <Space wrap>
          <Button type="info">Info</Button>
          <Button type="success">Success</Button>
          <Button type="warning">Warning</Button>
          <Button type="error">Error</Button>
      </Space>
  </Space>
<div class="box">
  <Carousel v-model="value" loop>
        <CarouselItem v-for="item in 5" :key="item">
            <div class="demo-carousel">
              <img class="food" :src="require('@/assets/images/green-food-1.jpg')">  
            </div>
        </CarouselItem>
     
    </Carousel>
</div>
 
</template>

<style lang="scss">
.food{
  width: 0vw;
}
</style>


<script>
    export default {
        data () {
            return {
                value: 0
            }
        }
    }
</script>