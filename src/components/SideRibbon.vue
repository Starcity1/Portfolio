<template>
    <div class="ribbon-main">
        <div>About Me</div>
        <div>Research</div>
        <div>Projects</div>
        <div>Singapore</div>
    </div>
</template>
<script>
    export default {
        name: "SideRibbon",
        data () {},
    }
</script>
<style>
    .ribbon-main {
        float: left;
        position: absolute;
        top: 0;
        left: 0;
        background: black;
        color: white;
        z-index: -10;
        width: 15vw;
        height: 100%;
        padding: 20px 20px 0px 20px;
        overflow-y: hidden;
    }
</style>