<template>
    <button class="post-button">Ver Detalle</button>
</template>

<script lang="ts">
    import { defineComponent, DefineComponent } from 'vue';

    export default defineComponent({
        name: "PostButton"
    })
</script>

<style lang="scss" scoped>
.post-button {
    background-color: aqua;
    padding: 3px;
    border: solid 1px blue;
    &:hover{
        background-color: blue;
        border: solid px aqua;
        color: #FFFFFF;
    }
}
</style>