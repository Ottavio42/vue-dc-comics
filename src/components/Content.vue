<template>
<div class="content">
    <div class="content-cont">
        -- Content goes here --
    </div>
</div>
</template>

<script>
export default {
    name: "Content"

}
</script>

<style lang="scss" scoped>

@import "../assets/style/variables";

.content{
    height: 5rem;
    background-color: #1c1c1c;
    .content-cont{
        font-size: 1.375rem;
        color: #fff;
        width: $sizeContainer;
        margin: auto;
    }
}
</style>