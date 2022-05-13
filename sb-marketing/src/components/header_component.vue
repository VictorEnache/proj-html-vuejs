<template>
    <header id="header">
        <div class="container">
            <div class="row">
                <Logo />
                <div class="nav_left d_flex">
                    <Navbar />
                    <Search />
                    <Cart />
                    <Button text='Get Started'/>
                </div>
            </div>
        </div>
    </header>
</template>
<!-- /template------------------------------------------------------------ -->


<script>
import Logo from './logo_component.vue'
import Navbar from './navbar_component.vue'
import Search from './search_component.vue'
import Cart from './cart_component.vue'
import Button from './button_component.vue'

export default {
    name:'header_component',

    components:{
        Logo,
        Navbar,
        Search,
        Cart,
        Button
    }
}
</script>
<!-- /script---------------------------------------------------------------- -->


<style lang="scss">
#header{
    padding: 10px 0;
    .container{
        .row{
            justify-content: space-between;
            align-items: center;
            .nav_left{
                align-items: center;

                #search{
                    margin: 0 20px;
                }

                #cart{
                    margin-right: 40px;
                }
            }
        }
    }
}
</style>
<!-- /style---------------------------------------------------------------- -->
