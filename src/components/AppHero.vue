<script>
export default {
    data(){
        return{
            image: "vue.svg"
        }
    },
    methods: {
        getIamge(path){
            return new URL(path, import.meta.url).href
        }
    },
}
</script>

<template lang="">
    <div>
        <img :src="getIamge(`../assets/${image}`)" width="150px">
    </div>
</template>
<style lang="">
    
</style>