<template>
    <div id="tip">
        <div class="tip_image">
            <div class="image">
                <img :src="img_src" alt="">
            </div>
        </div>
        <div class="tip_text">
            <h4>{{heading_text}}</h4>
            <p>Its a long etablished fact that a reader will be distracted by the readable content of a page when looking at its layout.</p>
        </div>
        <!-- /.tip_text -->
    </div>
    <!-- /#tip -->
</template>

<script>
export default {
    name:'tip_component',

    props:{
        heading_text: String,
        img_src: String
    }
}
</script>