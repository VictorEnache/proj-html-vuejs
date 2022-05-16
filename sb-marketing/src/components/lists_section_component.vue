<template>
    <div id="lists_section">
        <div class="container">
            <div class="row">
                <List />
                <List />
                <List />
            </div>
            <!-- /.row -->

        </div>
        <!-- /.container -->
    </div>
    <!-- /.lists -->
</template>



<script>
import List from './list_component.vue'

export default {
    name:'lists_section_component.vue',

    components:{
        List
    }
}
</script>

<style lang="scss">
    #lists_section{
        margin-top: 90px;
    }
</style>