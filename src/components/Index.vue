<template>
    <div class="wrapper">
        <Loading />       
        <Logo />
        <Cards />
    </div>
</template>

<style>

</style>

<script>
import Loading from './index/Loading.vue'
import Logo from './index/Logo.vue'
import Cards from './index/Cards.vue'
export default {
    name:'IndexHorizontal',
    components: {
        Loading,
        Logo,
        Cards
    },
    mounted() {
        Loading.activate()
        Logo.activate()
    }
}
</script>