<template>
    <nav id="vertical_nav">
        <div class="nav_name">
            {{nav_name}}
        </div>
        <ul>
            <li :key="index" v-for="(link,index) in links_array"><a href="#">{{link}}</a></li>
        </ul>
    </nav>
</template>



<script>
export default {
    name:'vertical_nav_component',

    props:{
        nav_name:String,
        links_array:Array
    }
}
</script>

<style lang="scss">
    #vertical_nav{
        padding-left: 2rem;
        .nav_name{
            font-size: 13px;
            font-weight: 600;
        }
        ul{
            
            li{
                a{
                    font-size: 12px;
                    color: $text-color-eta;
                }
            }
        }
    }
</style>