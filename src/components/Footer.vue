<template>
<footer>
    <div class="footer-top">
        <div class="foot-cont"></div>
    </div>
    <div class="footer-bot">
        <div class="foot-cont"></div>
    </div>
</footer>
</template>

<script>
export default {
    name: "Footer"

}
</script>

<style lang="scss" scoped>

@import "../assets/style/variables";

footer{
    height: 20rem;
    
    .footer-top {
        color: #fff;
        height: 70%;
    }
    .footer-bot{
            color: #fff;
            background-color: #303030;
            height: 30%;
        }
    .foot-cont{
            width: $sizeContainer;
        }

}
</style>