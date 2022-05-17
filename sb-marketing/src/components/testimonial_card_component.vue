<template>
    <div id="testimonial_card">
        <div class="info">
            <div class="image">
                <img :src="img_src" alt="">
            </div>
            <div class="text_container">
                <div class="name">
                    {{nome}} <span> - {{ruolo}}</span>
                </div>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestiae minima corporis, ea velit pariatur accusantium sequ</p>
            </div>
        </div>
        <!-- /.info -->
        <div class="secondo_strato"></div>
        <div class="terzo_strato"></div>
    </div>
    <!-- /#testimonial_card -->
</template>



<script>
export default {
    name:'testimonial_card_component',

    props:{
        img_src: String,
        nome: String,
        ruolo: String
    }
}
</script>


<style lang="scss">
    #testimonial_card{
        position: relative;
        width: 370px;
        height: 250px;
        .info{
            position: relative;
            z-index: 3;
            border-radius: 3px;
            background-color: white;
            height: 100%;
            box-shadow: -5px 5px 10px 2px $text-color-eta;
            .text_container{
                .name{
                    text-align: center;
                    span{
                        font-size: 12px;
                        color: $text-color-eta;
                    }
                }
                p{
                    padding: 21px;
                }
            }
            .image{
                width: 47px;
                margin: auto;
                padding: 33px 0;
                
    
                img{
                    width: 100%;
                    object-fit: cover;
                    border-radius: 50%;
                }
            }

        }
        .secondo_strato{
            border-radius: 3px;
            z-index: 2;
            background-color: white;
            width: calc(100% - 30px);
            height: 100%;
            position: absolute;
            top: 9px;
            left: 15px;
            box-shadow: 0px 5px 10px 2px $text-color-eta;
        }

            .terzo_strato{
            border-radius: 3px;
            background-color: white;
            width: calc(100% - 60px);
            height: 100%;
            position: absolute;
            top: 18px;
            left: 30px;
            box-shadow: 0px 5px 10px 2px $text-color-eta;
        }
    }
</style>