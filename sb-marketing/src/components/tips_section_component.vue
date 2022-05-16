<template>
    <section id="tips">
        <div class="container">
            <div class="row">
                <div class="tips_text col">
                    <h2>Get tips trick on how to skyrocket your sales</h2>
                    <p>Faff only about a quid blower i don't want no agro bleeding chimney pot burke tosser cras nice one boot fanny.!</p>
                    <Tip heading_text="Reporting analysis" :img_src="require('../assets/img/510.png')"/>
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
            .col{
                width: 50%;
            }

            .tips_img{
                background-image: url('../assets/img/509.jpeg');
                background-size: contain;
                background-position: bottom;
                background-repeat: no-repeat;
            }
        }
    }
}
</style>