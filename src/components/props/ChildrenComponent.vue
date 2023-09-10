<template>
    <div>
        {{ name }} 입니다
    </div>
    <button v-on:click="onChange">이름변경</button>
</template>

<script>
// import {ref} from 'vue';
    export default {
        props:['name', 'onChange'],
        setup (){
            
        }
    }
</script>