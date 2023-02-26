<template>
    <div>
        <h1 ref='tittle' v-text='111'></h1>
        <h2 v-text='222'></h2>
        <School ref="sch"/>
        <button @click="showDOM">点我展示DOM</button>
    </div>
</template>

<script>
import School from './components/School'
export default {
    name: 'App',
    components:{
        School
    },
    methods: {
        showDOM(){
            console.log(this.$refs)
        }
    },
};
</script>