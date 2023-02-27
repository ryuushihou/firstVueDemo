<template>
    <div>
        <h1 v-text="msg"></h1>
        <h2>姓名：{{name}}</h2>
        <h2>年龄：{{myAge+1}}</h2>
        <h2>性别：{{sex}}</h2>
        <button @click="addAge">点我年龄加1</button>
    </div>
</template>

<script>
export default {
    name: 'Student',
    data() {
        return {
            msg:'傻逼一中的学生',
            myAge:this.age
        }
    },
    methods: {
        addAge(){
            this.myAge++
        }
    },
    props:{
        name:String,
        age:Number,
        sex:String
    }
}
</script>