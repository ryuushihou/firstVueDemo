<template>
    <div class="demo">
        <h2>学校名字：{{name}}</h2>
        <h2>学校地址：{{address}}</h2>
    </div>
</template>

<script>
export default {
    name: 'School',
    data() {
        return {
            name:'傻逼一中',
            address:'密山'

        }
    }
}
</script>

<style>
    .demo{
        background-color: gray;
    }
</style>