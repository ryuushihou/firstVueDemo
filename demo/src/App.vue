<template>
    <div>
        <Student name="章三" sex="男" :age="18"/>
    </div>
</template>

<script>
import Student from './components/Student'
export default {
    name: 'App',
    components:{
        Student
    }
};
</script>