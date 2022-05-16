<template>
    <div id="list" class="row">
        <div class="list_img">
            <div class="image">
                <img src="../assets/img/24.png" alt="">
            </div>
        </div>
        <!-- /.list_img -->
        <div class="list_text">
            <h3>Online Marketing</h3>
            <p>It is a long estabilished fact that a reader will be distracted.</p>
            <ul>
                <li :key='index' v-for='(string,index) in list_content'>
                    <span class="check_icon">
                        <fa-icon :icon="['fas', 'check']" />
                    </span>
                    {{string}}
                </li>
            </ul>
        </div>
        <!-- /.list_text -->
    </div>
    <!-- /.list -->
</template>



<script>
export default {
    name:"list_component",

    data(){
        return{
            list_content:['SEO', 'SEM', 'Website Strategy', 'Social Management']
        }
    }
}
</script>

<style lang="scss">
    #list{
        flex-basis: 0;
        flex-grow: 1;
        .list_img{
            padding: 0 22px;
            .image{
                width: 55px;
            }

            img{
                width: 100%;
                object-fit:fill;
            }
        }

        .list_text{
            
            ul{
                padding-top: 22px;
                li{
                    line-height: 28px;
                    font-size: 11px;
                    font-weight: 600;
                    .check_icon{
                        color: $text-color-epsilon;
                        font-size: 900;
                    }
                }
            }
        }
    }
</style>