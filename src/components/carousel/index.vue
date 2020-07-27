<template>
  <el-carousel height="560px">
      <el-carousel-item v-for="(item) in data" :key="item.url">
          <a><img :src="item.url"/></a>
      </el-carousel-item>
  </el-carousel>
</template>

<script>
export default {
  data() {
    return {
      data: [
        {
          url: require("@/assets/image/carousel1.jpg"),
          path: ''
        },
        {
          url: require("@/assets/image/carousel2.jpg"),
          path: ''
        },
        {
          url: require("@/assets/image/carousel3.jpg"),
          path: ''
        },
      ]
    }
  },
  mounted() {

  }
}
</script>

<style scoped>
  img {
    width: 100%;
    height: 560px;
  }
</style>