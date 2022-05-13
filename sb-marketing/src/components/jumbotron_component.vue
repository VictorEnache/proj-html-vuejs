<template>
    <section id="hero_image">
        <div class="hero_container d_flex">
            <div class="col-6">
                <h1>The biggest platform for your growth.</h1>
                <p>
                    There are many variations of passages of lorem ipsum available, but the majority
                    have suffered alteration in some form
                </p>
                <Button_c text="Read More" />
            </div>
            <div class="col">
                <img src="../assets/img/27-1.png" alt="">
            </div>
            <!-- /.col-8 -->
        </div>
    </section>
    <!-- /#hero_image -->
</template>



<script>
import Button_c from './button_component.vue'

export default {
    name:'jumbotron_component',

    components:{
        Button_c
    }
}
</script>

<style lang="scss">
    #hero_image{
        margin-top: 10px;
        .hero_container{
            width: 1050px;
            margin: auto;
            background: linear-gradient( $bg-color-beta, $bg-color-beta 90%, #fff 50%);
            

            .col-6{
                width: calc(100% * 6/12);
                padding: 45px 0 45px 45px;

                h1{
                    font-size: 40px;
                    margin-bottom: 1rem;
                }

                p{
                    font-size: 13px;
                    margin-bottom: 2rem;
                }
            }

            .col{
                padding-top: 20px;
                
                img{
                    width: 100%;
                    object-fit: cover;
                }
            }
        }
    }
</style>