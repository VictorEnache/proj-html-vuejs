<template>
    <main id="site_main">
        <Hero_image />
        <Lists/>
        <Tips/>
        <Features/>
        <Testimonials />
        <Latest_posts />
    </main>
    <!-- /#site_main -->
</template>



<script>
import Hero_image from './jumbotron_component.vue'
import Lists from './lists_section_component.vue'
import Tips from './tips_section_component.vue'
import Features from './features_section_component.vue'
import Testimonials from './testimonials_section_component.vue'
import Latest_posts from './latest_posts_component.vue'

export default {
    name:'main_component',

    components:{
        Hero_image,
        Lists,
        Tips,
        Features,
        Testimonials,
        Latest_posts
    }
}
</script>



<style lang="scss">

</style>