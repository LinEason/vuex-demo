<template>
    <div>
        <p>这是 HelloVuex组件</p>
        <hr>
        {{ storeMes  }}
    </div>
</template>
<script>
export default {
    name:"HelloVuex",
    created(){
        //console.log(this.$store.state.count);
        this.storeMes = this.$store.state.count;
    }
}
</script>
<style lang="">
    
</style>