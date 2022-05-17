<template>
    <div id="feature_card">
        <h4>{{title}}</h4>
        <div class="image">
            <fa-icon :icon="array_icona" :class='colore'/>
        </div>
    </div>
    <!-- /#feature_card -->
</template>

<script>
export default {
    name:'feature_card_component',

    props:{
        array_icona: Array,
        title: String,
        colore: String
    }
}
</script>


<style lang="scss">
    #feature_card{
        padding: 1rem;
        border-radius: 5px;
        width: calc(100% / 4 - 22px + 22px/4);
        height: 116px;
        box-shadow: 0 0 20px 15px $bg-color-beta;
        .image{
            font-size: 35px;

            .blue{
                color: $text-color-epsilon;
            }

            .red{
                color: $text-color-gamma;
            }

            .green{
                color: $text-color-beta;
            }
            
        }
        
    }
</style>