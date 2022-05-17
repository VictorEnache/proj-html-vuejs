<template>
    <section id="tips">
        <div class="container">
            <div class="row">
                <div class="tips_text col">
                    <div class="upper_text">

                        <h2>Get tips trick on how to skyrocket your sales</h2>
                        <p>Faff only about a quid blower i don't want no agro bleeding chimney pot burke tosser cras nice one boot fanny.!</p>
                    </div>
                    <Tip heading_text="Reporting analysis" :img_src="require('../assets/img/510.png')" class="active"/>
                    <Tip heading_text="Thecnical SEO Audit" :img_src="require('../assets/img/511.png')"/>
                </div>
                <!-- /.tips_text -->
                <div class="tips_img col">
                </div>
                <!-- /.tips_img -->
            </div>
            <!-- /.row -->
        </div>
    </section>
    <!-- /#tips -->
</template>



<script>
import Tip from './tip_component.vue'

export default {
    name:'tips_section_component',

    components:{
        Tip
    }
}
</script>


<style lang="scss">
#tips{
    margin-top: 110px;
    .container{
        .row{
            column-gap: 1rem;
            .col{
                width: 50%;
            }

            .tips_img{
                background-image: url('../assets/img/509.jpeg');
                background-size: contain;
                background-position: bottom;
                background-repeat: no-repeat;
            }

            .tips_text{
                .active{
                    border: 1px solid $border-color-beta;
                    box-shadow: 10px 20px 25px $border-color-beta;
                }
                .upper_text{
                    padding-bottom: 30px;
                }
            }
        }
    }
}


</style>