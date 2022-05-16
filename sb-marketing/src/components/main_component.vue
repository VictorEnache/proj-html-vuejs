<template>
    <main id="site_main">
        <Hero_image />
        <Lists/>
        <Tips/>
    </main>
    <!-- /#site_main -->
</template>



<script>
import Hero_image from './jumbotron_component.vue'
import Lists from './lists_section_component.vue'
import Tips from './tips_section_component.vue'

export default {
    name:'main_component',

    components:{
        Hero_image,
        Lists,
        Tips
    }
}
</script>



<style lang="scss">

</style>