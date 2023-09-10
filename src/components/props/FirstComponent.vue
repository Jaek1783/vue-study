<template>
    <Children :name="name" :onChange="onChange"/>
</template>

<script>
import {ref} from 'vue'
import Children from './ChildrenComponent.vue'
export default {
    components: {
    Children
  },
    setup() {
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