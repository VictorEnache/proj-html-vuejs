<template>
    <header id="#header">
        <div class="container">
            <Logo />
            <Navbar />
            <Search />
            <Cart />
        </div>
    </header>
</template>
<!-- /template------------------------------------------------------------ -->


<script>
import Logo from './logo_component.vue'
import Navbar from './navbar_component.vue'
import Search from './search_component.vue'
import Cart from './cart_component.vue'

export default {
    name:'header_component',

    components:{
        Logo,
        Navbar,
        Search,
        Cart
    }
}
</script>
<!-- /script---------------------------------------------------------------- -->


<style lang="scss">

</style>
<!-- /style---------------------------------------------------------------- -->
