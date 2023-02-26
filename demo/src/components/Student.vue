<template>
    <div class="demo">
        <h2>{{stuName}}</h2>
        <h2>{{stuEngName}}</h2>
    </div>
</template>

<script>
export default {
    data(){
        return{
            stuName:'小红',
            stuEngName:'xiaohong'
        }
    }
}
</script>

<style>
    .demo{
        background-color: orange;
    }
</style>