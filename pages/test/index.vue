<template>
    <div class="mb-10">
    <h1  @click="changeText">{{jr}}</h1>
  </div>
</template>

<script>
export default {
    props:{
        title:{
            type: String
        }
    },
    data(){
        return {
            jr:'Click me'
        }
    },
    methods:{
        changeText: function(){
            this.$emit('changeText', 'yey');
        }
    }
}
</script>

<style>
.mb-10 {
    padding-top: 150px;
}
</style>