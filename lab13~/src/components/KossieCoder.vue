<template>
    <div>
        <h1>{{ title }}</h1>
        <p>{{ name }}</p>
        <button @click="updateName">Change Name</button>
    </div>

</template>

<script>
export default {
    // props: ['title'], 이 방법도 있고
    props: {
        title:{
            type: String,
            default: 'default title',
            required: false
        },
        name:{
            type: String,
            default: 'default title',
        }
    },
    data(){
        return{
            // name: 'Kossie Coder',
        }
    },
    methods: {
        updateName(){
            // 자식이 부모에게서 오는 props 내용을 변경하지 않아야 함, 다이아몬드 문제
            this.name = 'Kossie Coder Updated';
        }
    }
}
</script>
<style scoped>

</style>