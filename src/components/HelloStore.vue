<template>
    <div>
        <p>这是 HelloStore组件</p>
        <hr>
        {{ storeMes  }}
        {{storeMes1}}
        <hr>
        <button @click="storeChange">commit</button>
    </div>
</template>
<script>
    export default {
        name:"HelloStore",
        data(){
            return{
                storeMes: ''
            }
        },
        computed:{
            //storeMes1 : this.$store.state.count
            //storeMes: this.$store.state.count
            storeMes1(){
                return this.$store.state.count
            }
        },
        methods:{
            storeChange(){
                this.$store.commit('increment');
                //alert(1)
            }
        },
        created(){
            //console.log(this.$store.commit);
            this.storeMes = this.$store.state.count;
        }
    }
</script>
<style lang="">
    
</style>