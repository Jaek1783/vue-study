<template>
    <h2>toRefs, reactive 학습</h2>
    <div>
        <span>생선 이름 : {{ name }}</span>

        <span>가격 : {{ price }}</span>
    </div>
    <button @click="change">생선 바꾸기</button>
    <hr/>
</template>

<script>
import {reactive, toRefs} from 'vue';
export default {
    setup(){
        const change = ()=>{
            fish.name = '갈치 ',
            fish.price = 1000
        }
        const fish = reactive({
            name : '고등어 ',
            price : 5000
        });

        return {
            ...toRefs(fish),
            change
        }
    }
}
</script>