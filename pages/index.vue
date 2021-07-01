<template>
  <el-main class="overflow-hidden">
    <ovalsTop>
      <img src="/stars/star1.svg" class="star star-left">
      <img src="/stars/star3.svg" class="star star-center">
      <img src="/stars/star2.svg" class="star star-right">
    </ovalsTop>
    <el-card 
      class="box-card card-border-radius h-100 border-0 regular-card-heigth relative"
      :body-style="{ height: '100%' }"
    >
      <img src="/figures/triangle.svg" class="figure figure-triangle absolute">
      <img src="/figures/oval.svg" class="figure figure-oval absolute">
      <img src="/figures/oval-bold.svg" class="figure figure-oval-bold absolute">
      <img src="/figures/rectangle.svg" class="figure figure-rectangle absolute">
      <div class="d-flex direction-column justify-between h-100">
        <div>
          <img src="/man.png" alt="" class="m-auto mt-15 d-block">
          <h1 class="text-center base-font base-font-bold">Glad to see you!</h1>
          <p class="text-center base-font">
            To give you the most accurate prediction, I need to know some information about you.
          </p>
          <img src="/shield.svg" alt="" class="m-auto mt-15 d-block">
          <p class="text-center base-font">
            Don't worry, all the information is protected and will be saved on your device.
          </p>
        </div>
        <div class="w-100 d-flex justify-center text-center mb-50">
          <el-button 
            @click="moveTo('/name')"
            class="base-button base-font base-font-bold base-font-size text-center text-white uppercase border-0 z-index-1 relative"
          >
            Get started
          </el-button>
        </div>
      </div>

      <ovalsBottom />
    </el-card>
  </el-main>
</template>

<script>
import global from '~/mixins/global'
import ovalsTop from '~/components/ovals-top'
import ovalsBottom from '~/components/ovals-bottom'

export default {
  layout: 'orange',
  mixins: [global],
  components: {
    ovalsTop,
    ovalsBottom
  }
}
</script>
