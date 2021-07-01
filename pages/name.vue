<template>
  <el-main>
    <el-card 
      class="box-card card-border-radius h-100 border-0 regular-card-heigth relative mt-75"
      :body-style="{ height: '100%' }"
    >
      <div class="d-flex direction-column justify-between h-100">
        <div>
          <img src="/man-stands.png" alt="" class="m-auto mt-15 d-block">
          <h1 class="text-center base-font base-font-bold">
            For starters, let's get to know each other.
          </h1>
        </div>
        <div class="w-100 text-center mb-50">
          <div class="w-100">
            <el-input
              v-model="name"
              placeholder="Type your Name"
              class="base-input border-0 mb-15 z-index-1" 
            />
          </div>
          <div class="w-100">
            <el-button
              class="base-button base-font base-font-bold base-font-size text-center text-white uppercase border-0 z-index-1 relative"
            >
              Continue
            </el-button>
          </div>
        </div>
      </div>
      <ovalsBottom />
      <ovalsOrange />
    </el-card>
  </el-main>
</template>

<script>
import ovalsBottom from '~/components/ovals-bottom'
import ovalsOrange from '~/components/ovals-orange'

export default {
  layout: 'orange',
  components: {
    ovalsBottom,
    ovalsOrange
  },
  data(){
    return{
      name: ''
    }
  }
}
</script>

<style lang="scss" scoped>

</style>
