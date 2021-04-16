<template>
    <div>
        <h1 ref="myref">Hook</h1>
        <h2>My name is: {{name}}</h2>
    </div>
</template>

<script>
export default ({
    data() {
        return{
            name: 'bakir'
        }
    },

    beforeCreate(){
        console.log(this.name)
    },

    created(){
        console.log('data and other function is available but not html', this.name)
    },
    mounted(){
        console.log(this.$refs.myref)
    }
})
</script>
