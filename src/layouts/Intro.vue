<template lang="html">
  <q-layout class="bg-light-blue-13">
    <div class="fixed-center full-width q-pa-xl text-white text-h6 text-center">
      Welcome to GAME-UI
      <q-spinner-pie
        color="white"
        size="50vw"
        class="q-mt-xl"
      />
    </div>
  </q-layout>
</template>

<script>
import { VueRouter } from 'vue-router'
import { useQuasar, QSpinnerPie } from 'quasar'

export default {
  setup(){
    const $router = useQuasar(VueRouter)
    return{
      QSpinnerPie
    }
  },
  mounted(){
    setTimeout(()=>{
          this.$router.push('main')
    },2500)

  }
}
</script>

<style lang="css" scoped>
</style>
