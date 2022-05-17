<template>
    <div id="form">
        <h4>Get in Touch</h4>
        <div class="row">
            <input id="name" type="text" placeholder="Your Name">
            <input id="email" type="email" placeholder="Your Email">
            <input id="subject" type="text" placeholder="Your Subject">
            <textarea id="message" rows="7" placeholder='Your Message'></textarea>
        </div>
        <!-- /.row -->
    </div>
    <!-- /#form -->
</template>


<script>
export default {
    name:'form_component'
}
</script>



<style lang="scss">
    #form{

        .row{
            padding-top: 22px;
            flex-wrap: wrap;
            row-gap: 22px;

            #name,
            #email{
                width: calc(50% - 11px);
                height: 35px;
                border: 1px solid $bg-color-beta;
            }
            #subject{
                width: 100%;
                height: 35px;
                border: 1px solid $bg-color-beta;
            }
            #message{
                width: 100%;
                height: 165px;
                border: 1px solid $bg-color-beta;
            }

         
        }
    }
</style>