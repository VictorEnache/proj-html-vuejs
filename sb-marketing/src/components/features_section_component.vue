<template>
    <section id="features">
        <div class="container">
            <div class="row">
                <div class="features_text">
                    <h2>Popular features that your business needs</h2>
                    <p>Faff only about a quid blower i don't want no agro bleeding chimney pot burke tosser cras nice one boot fanny.!</p>
                </div>
                <!-- /.features_text -->
                <div class="button">
                    <Button text="Explore More Feature" />
                </div>
            </div>
            <!-- /.row -->
            <div class="card_container">
                <div class="row">
                    <Feature_card :key='index' v-for='(card,index) in feature_cards' :array_icona="card.icon" :title="card.title" :colore="card.color"/>
                </div>

            </div>
        </div>
        <!-- /.container -->
    </section>
    <!-- /#features -->
</template>

<script>
import Button from './button_component.vue'
import Feature_card from './feature_card_component.vue'

export default {
    name:'features_section_component',

    components:{
        Button,
        Feature_card
    },

    data(){
        return{
            feature_cards:[
                {
                    title:'Customized Invoices',
                    icon:['fas', 'chart-line'],
                    color:'blue'
                },
                {
                    title:'Stock Managment',
                    icon:['fas', 'paper-plane'],
                    color:'red'
                },
                {
                    title:'Receivable & payables',
                    icon:['fas', 'user-gear'],
                    color:'green'
                },
                {
                    title:'Manage Buying',
                    icon:['fas', 'user-plus'],
                    color:'blue'
                },
                {
                    title:'Powerfull & Secure',
                    icon:['fas', 'circle-nodes'],
                    color:'red'
                },
                {
                    title:'Fastest Return Filing',
                    icon:['fas', 'user-gear'],
                    color:'green'
                },
                {
                    title:'Monthly Detailed',
                    icon:['fas', 'file-pen'],
                    color:'blue'
                },
                {
                    title:'Product Managment',
                    icon:['fas', 'thumbs-up'],
                    color:'red'
                }
            ]
        }
    }
}
</script>


<style lang="scss">
    #features{
        margin-top: 100px;
        .container{
            .row{
                .features_text{
                    p{
                        width: calc(100% * 2/3);
                    }
                }
                justify-content: space-between;
                .button{
                    padding-right: 35px;
                    padding-top: 35px;
                }
            }
            .card_container{
                margin-top: 40px;
                .row{
                    flex-wrap: wrap;
                    row-gap: 22px;
                }
            }
        }
    }
</style>
