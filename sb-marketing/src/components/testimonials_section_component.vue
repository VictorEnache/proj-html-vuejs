<template>
    <section id="testimonials">
        <div class="container">
            <div class="testimonials_text">
                <h2>Our Testimonials</h2>
                <p>If you are planning on developing a product landing app or website, take a look at this beautiful-crafted</p>
            </div>
            <!-- /.testimonials_text -->
            <div class="testimonial_cards row">
                <Testimonial_card :img_src="persona.image" :nome="persona.nome" :ruolo="persona.ruolo" :key='index' v-for="(persona, index) in people"/>
            </div>

            <div class="pallini">
                <fa-icon :icon="['fas','circle']"/>
                <fa-icon :icon="['fas','circle']"/>
            </div>
            <!-- /.testimonial_cards -->
        </div>
    </section>
    <!-- /#testimonials -->
</template>



<script>
import Testimonial_card from './testimonial_card_component.vue'

export default {
    name:'testimonials_section_component',

    data(){
        return{
            people:[
                {
                    nome:'Julia Aann',
                    ruolo:'COO softbox',
                    image:require("../assets/img/26.jpeg")
                },
                                {
                    nome:'Julia Aann',
                    ruolo:'COO softbox',
                    image:require("../assets/img/27.jpeg")
                }
            ]
        }
    },

    components:{
        Testimonial_card
    }
}
</script>



<style lang="scss">
    #testimonials{
        margin-top: 90px;
        .container{
            .testimonials_text{
                margin: auto;
                text-align: center;
                width: 50%;
            }

            .testimonial_cards{
                padding-top: 75px;
                padding-bottom: 2.5rem;
                justify-content: space-between;
            }

            .pallini{
                width: fit-content;
                margin: auto;
            }
        }
    }
</style>