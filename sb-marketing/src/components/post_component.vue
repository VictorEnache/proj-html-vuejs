<template>
    <div id="post_component">
        <div class="post_image">
            <div class="date">{{date}}</div>
            <img :src="img_src" alt="">
        </div>
        <div class="post_text">
            <h4>Life Lack Meaning</h4>
            <p>Its a long estabilished fact that a reader will be distracted by the readable</p>
        </div>
    </div>
    <!-- /#post_component -->
</template>



<script>
export default {
    name:'post_component',

    props:{
        img_src: String,
        date: String,

    }
}
</script>



<style lang="scss">
    #post_component{
        margin-top: 75px;
        width: 255px;
        border: 1px solid $bg-color-beta;
        padding: 7px;
        border-radius: 3px;

        .post_image{
            position: relative;

            .date{
                background-color: white;
                color: $text-color-eta;
                position: absolute;
                top: 7px;
                left: 7px;
                font-size: 12px;
                padding: 0.25rem;
                border-radius: 3px;
            }
            img{
                width: 100%;
                object-fit: cover;
            }
        }

        .post_text{
            padding: 1rem;
        }
    }
</style>