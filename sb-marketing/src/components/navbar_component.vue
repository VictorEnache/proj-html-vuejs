<template>
    <nav id="navbar">
        <ul class="row">
            <li v-for="(link,index) in navLinks" :key="index">
                <a href="#">{{link.name}}</a>
            </li>
        </ul>
    </nav>
    <!-- /#navbar -->
</template>



<script>
export default {
    name:'navbar_component',

    data(){
        return{
            navLinks:[{name:'Home'}, {name:'About us'}, {name:'Feature'}, {name:'Testimonials'}, {name:'Contact US'}]
        }
    }
}
</script>

<style lang="scss">
    #navbar{
        ul{
            li{
                margin: 0 10px;

                a{
                    color: $text-color-theta;
                    padding: 10px 0;
                    font-size: 12px;
                    font-weight: 600;

                    &:hover{
                        border-bottom: 2px solid $border-color-gamma;
                        color: $text-color-epsilon;
                    }
                }
            }
        }
    }
</style>