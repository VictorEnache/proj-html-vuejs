<template>
    <div id="button">
        <a href="#">{{text}}</a>
    </div>
    <!-- /#button -->
</template>



<script>
export default {
    name: 'button_component',

    props:{
        text: String
    }
}
</script>

<style lang="scss">
    #button{
        width: fit-content;

        a{
            background-color: $bg-color-gamma;
            border-radius: 3px;
            display: block;
            color: $text-color-alpha;
            text-decoration: none;
            font-size: 11px;
            padding: 11px 14px;
            
        
        }
    }
</style>