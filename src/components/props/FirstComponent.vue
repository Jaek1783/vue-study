<template>
    <div>
       <span>my name is '{{ name }}'</span> 
    </div>
</template>

<script>
export default {
    setup() {
        const name ='Choi_Jaekeun';
        return {
            name
        }
    }
}
</script>