<template>
    <h2>props 학습</h2>
    <div>
        {{ name }} 입니다
    </div>
    <button v-on:click="onChange">이름변경</button>
    <hr/>
</template>

<script>
// import {ref} from 'vue';
    export default {
        props:['name', 'onChange'],
        setup (){
            
        }
    }
</script>