<template>
    <section id="latest_posts">
        <div class="container">
            <div class="text">
                <h2>Latest Posts</h2>
                <p>If you are planning on developing a product landing</p>
            </div>
            <div class="row">
                <Post :key='index' v-for="(post, index) in posts" :img_src="post.image" :date="post.date"/>
            </div>
            <!-- /.row -->
        </div>
        <!-- /.container -->
    </section>
    <!-- /#latest_posts -->
</template>



<script>
import Post from './post_component.vue'

export default {
    name:'latest_posts_component',

    data(){
        return{
            posts:[
                {
                    image:require('../assets/img/17.jpg'),
                    date:'November 28, 2019'
                },
                {
                    image:require('../assets/img/18.jpg'),
                    date:'November 28, 2019'
                },
                {
                    image:require('../assets/img/19.jpg'),
                    date:'November 28, 2019'
                }
            ]
        }
    },

    components:{
        Post
    }
}
</script>

<style lang="scss">
    #latest_posts{
        margin-top: 90px;
        .container{
            .text{
                text-align: center;
            }
            .row{
                justify-content: space-around;
                
            }
        }
    }
</style>