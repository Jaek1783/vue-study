<template>
<h1>Vue 3.0 학습</h1>
<Children01 :name="name" :onChange="onChange"/>
</template>

<script>
import Children01 from './components/props/ChildrenComponent.vue';
import {ref} from 'vue';
export default {
  name: 'App',
  components: {
    Children01
  },
  setup (){
    const boolean = ref(true);
    const name = ref('최재근');
    const onChange = ()=>{
      boolean.value = !boolean.value;
      if(!boolean.value){
        name.value = '최재강'
      }else{
        name.value = '최재근'
      }
      console.log(boolean.value)
            }
    return {
      name,
      onChange
    }
  }
}
</script>

<style>
</style>
