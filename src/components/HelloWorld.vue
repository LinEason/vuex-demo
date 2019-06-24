<template>
    <div>
        <p>z这是hello word 组件</p>
        <hr>
        {{ storeMes  }}
    </div>
</template>

<script>
export default {
    name: 'HelloWorld',
    data () {
      return {
        msg: 'Welcome to Your Vue.js App'
      }
    },
    created(){
          //console.log(this.$store.state.count);
          this.storeMes = this.$store.state.count;
      }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
