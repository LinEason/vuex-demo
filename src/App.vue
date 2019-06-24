<template>
    <div>
      <HelloWorld></HelloWorld>
      <HelloVuex></HelloVuex>
      <HelloStore></HelloStore>
    </div>
</template>

<script>
    import HelloWorld from '@/components/HelloWorld'
    import HelloVuex from '@/components/HelloVuex'
    import HelloStore from '@/components/HelloStore'
    export default {
        data(){
            return {

            }
        },
        components : {
            HelloWorld,
            HelloVuex,
            HelloStore
        }
    }
</script>

<style>

</style>
