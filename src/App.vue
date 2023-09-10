<template>
  <h1>Vue 3.0 학습</h1>
  <Study01/>
  <Study02/>
</template>

<script>
import Study01 from './components/props/FirstComponent.vue'
import Study02 from './components/torefs/toRefsComponent.vue'
export default {
  name: 'App',
  components:{
    Study01,
    Study02
  },
  setup (){
    return {
    }
  }
}
</script>
