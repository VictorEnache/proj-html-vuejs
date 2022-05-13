<template>
    <header id="#header">
        <div class="container">
            <Logo />
            <Navbar />
        </div>
    </header>
</template>
<!-- /template------------------------------------------------------------ -->


<script>
import Logo from './logo_component.vue'
import Navbar from './navbar_component.vue'

export default {
    name:'header_component',

    components:{
        Logo,
        Navbar
    }
}
</script>
<!-- /script---------------------------------------------------------------- -->


<style lang="scss">

</style>
<!-- /style---------------------------------------------------------------- -->
