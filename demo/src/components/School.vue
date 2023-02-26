<template>
    <div>
        <h1 :style="{opacity}">这就是个傻逼demo</h1>
        <h2>{{name}}</h2>
        <h2>{{enName}}</h2>
        <button @click="showname">点我提示名字</button>
    </div>
</template>

<script>
export default {
    data(){
        return{
            name:'密山傻逼一中',
            enName:'mishanshabiyizhong',
            opacity:1
        }
    },
    methods: {
        showname(){
            alert(this.name)
        }   
    },
    mounted() {
        console.log('mounted',this)
				setInterval(() => {
					this.opacity -= 0.01
					if(this.opacity <= 0) this.opacity = 1
				},16)
    }
}
</script>