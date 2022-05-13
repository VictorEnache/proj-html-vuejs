<template>
    <div id="cart">
        <div class="cart_icon">
            <fa-icon :icon="['fas', 'cart-shopping']" />
        </div>
        <div class="count d_flex">
            <span class="number">0</span>
        </div>
    </div>
</template>



<script>
export default {
    name:'cart_template'
}
</script>



<style lang="scss">
    #cart{
        font-size: 12px;  
        position: relative;  
        width: fit-content; 

        .cart_icon{
            position: relative;
            z-index: 2;
        }
        
        .count{
            height: 15px;
            width: 15px;
            background-color: $bg-color-gamma;
            border-radius: 50%;
            justify-content: center;
            align-items: center;
            font-size: 10px;
            color: white;
            position: absolute;
            top: -40%;
            right: -70%;
            
        }
    }
</style>