<template>
    <footer id="site_footer">
        <div class="container">
            <div class="row">
                <div class="col">
                    <div class="logo d_flex">
                        <Logo />
                        <div class="logo_text">
                            SOFBOX
                        </div>
                    </div>
                    <p>It is a long etbilished fact that a reader will be distracted by the readable content.</p>

                    <div class="copyright">
                        copyright @ 2018 <span>sofbox</span>
                    </div>
                </div>
                <div class="col" :key='index' v-for='(nav,index) in nav_list'>
                    <Vertical_nav  :nav_name='nav.name' :links_array="nav.links_array"/>
                </div>
            </div>
        </div>
    </footer>
    <!-- /#site_footer -->
</template>

<script>
import Logo from './logo_component.vue'
import Vertical_nav from './vertical_nav_component.vue'

export default {
    name:'site_footer',

    components:{
        Logo,
        Vertical_nav
    },

    data(){
        return{
            nav_list:[
                {
                    name:'Menu',
                    links_array:['About us', 'Theme', 'Features', 'Pricing', 'Blog']
                },
                {
                    name:'About us',
                    links_array:['About sofbox', 'Roadmap', 'How it work', 'Team', 'News']
                },{
                    name:'quick Links',
                    links_array:['About us', 'Theme', 'Features', 'Pricing', 'Blog']
                }
            ]
        }
    }
}
</script>



<style lang="scss">
    #site_footer{
        border-top: 2px solid $bg-color-beta;
        padding: 55px 0;
        margin-top: 90px;
        .container{
            .row{
                .col{
                    width: calc(100% * 1/4);
                }
                .logo{
                    align-items: center;
                    font-size: 12px;
                    column-gap: 0.5rem;
                    color: $text-color-epsilon;
                }

                .copyright{
                    margin-top: 45px;
                    font-size: 12px;
                    color: $text-color-eta;

                    span{
                        color: $text-color-epsilon;
                    }
                }
            }
        }
    }
</style>