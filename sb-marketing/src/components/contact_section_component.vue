<template>
    <section id="contact_section">
        <div class="container">
            <div class="row">
                <div class="col mappa">
                    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2798.4056362213173!2d9.133478051181177!3d45.461632078998456!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x4786c22ab05c3bbf%3A0xa481aa5be8d54a11!2sBoolean%20SRLS!5e0!3m2!1sit!2sit!4v1652795722086!5m2!1sit!2sit"  style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
                </div>
                <!-- /.col -->
                <div class="col ">
                    <div class="contatti d_flex">
                        <Logo />
                        <div class="text_logo">
                            SOFBOX
                        </div>

                    </div>
                    <!-- /.contatti -->
                </div>
                <!-- /.col -->
            </div>
            <!-- /.row -->
        </div>
        <!-- /.container -->
    </section>
    <!-- /.contact -->
</template>



<script>
import Logo from './logo_component.vue'

export default {
    name:'contact_section_component',

    components:{
        Logo
    }
}
</script>



<style lang="scss">
    #contact_section{
        margin-top: 90px;
        .container{
            .row{
                column-gap: 22px;
                .col{
                    width: 50%;
                }
                .mappa{
                    iframe{
                        width: 100%;
                        height: 325px;
                    }
                }

                .contatti{
                    align-items: center;
                    column-gap: 0.5rem;
                    .text_logo{
                        color: $text-color-epsilon;
                        font-size: 12px;
                        font-weight: 600;
                    }
                }
                
            }
        }
    }
</style>