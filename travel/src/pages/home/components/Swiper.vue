<template>
  <div>
    <div class="wrapper">
      <swiper :options="swiperOption">
        <swiper-slide v-for="item of swiperList"
                      :key="item.id">
          <img class="swiper-img"
               :src="item.imgUrl"
               alt="">
        </swiper-slide>
        <div class="swiper-pagination"
             slot="pagination"></div>
      </swiper>
    </div>
  </div>

</template>
<script>
export default {
  name: 'HomeSwiper',
  data() {
    return {
      swiperOption: {
        pagination: '.swiper-pagination',
        loop: true
      },
      swiperList: [
        {
          id: '0001',
          imgUrl: '//img1.qunarzz.com/qs/1811/3f/85a00499e2e0802.jpg'
        },
        {
          id: '0002',
          imgUrl: '//img1.qunarzz.com/qs/1809/64/62160a38d119c202.jpg'
        }
      ]
    }
  }
}
</script>
<style lang="stylus" scoped>
.wrapper >>> .swiper-pagination-bullet-active
  background #fff
.wrapper
  overflow hidden
  width 100%
  height 0
  padding-bottom 25.6%
  background #eeeeee
  .swiper-img
    width 100%
</style>
