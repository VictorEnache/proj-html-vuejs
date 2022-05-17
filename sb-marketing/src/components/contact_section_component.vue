<template>
    <section id="contact_section">
        <div class="container">
            <div class="row">
                <div class="col mappa">
                    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2798.4056362213173!2d9.133478051181177!3d45.461632078998456!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x4786c22ab05c3bbf%3A0xa481aa5be8d54a11!2sBoolean%20SRLS!5e0!3m2!1sit!2sit!4v1652795722086!5m2!1sit!2sit"  style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
                </div>
                <!-- /.col -->
                <div class="col contatti">
                    <div class=" logo d_flex">
                        <Logo />
                        <div class="text_logo">
                            SOFBOX
                        </div>

                    </div>
                    <!-- /.logo -->
                    <div class="indirizzo">
                        Piazzale Giovanni delle Bande Nere, 9, 20146 Milano MI
                    </div>
                    <!-- /.indirizzo -->
                    <div class="numero">
                        0240 031 288
                    </div>
                    <!-- /.numero -->
                    <div class="email">
                        imail@sofbox.com
                    </div>
                    <!-- /.email -->
                    <div class="social row">
                        <div class="facebook">
                            <fa-icon :icon="['fas', 'user']" />
                        </div>
                        <div class="twitter">
                            <fa-icon :icon="['fas', 'user']" />
                        </div>
                        <div class="github">
                            <fa-icon :icon="['fas', 'user']" />
                        </div>
                        <div class="instagram">
                            <fa-icon :icon="['fas', 'user']" />
                        </div>
                    </div>

                    <Form/>
                    <Button text="Send Message"/>
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
import Form from './form_component.vue'
import Button from './button_component.vue'

export default {
    name:'contact_section_component',

    components:{
        Logo,
        Form,
        Button
    }
}
</script>



<style lang="scss">
    #contact_section{
        #button{
            padding-top: 22px;
        }
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
                    .logo{
                        align-items: center;
                        column-gap: 0.5rem;
                        padding-bottom: 22px;

                    }
                    .text_logo{
                        color: $text-color-epsilon;
                        font-size: 12px;
                        font-weight: 600;
                    }

                    .indirizzo{
                        padding: 22px 0;
                        color: $text-color-eta;
                    }

                    .email{
                        padding: 22px 0;
                        color: $text-color-eta;
                    }

                    .social{
                        padding: 22px 0;
                    }

                    .social>*{
                        display: flex;
                        align-items: center;
                        justify-content: center;
                        height: 30px;
                        width: 30px;
                        border: 1px solid $bg-color-beta;
                        font-size: 11px;
                        color: $text-color-epsilon;
                    }
                    
                }
                
            }
        }
    }
</style>