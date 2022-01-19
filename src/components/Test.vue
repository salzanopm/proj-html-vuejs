<template>
<div>
    <h2 class="static-class" :class="{green:colorfull}">CIAO</h2>
    <button v-on:click="colorfull=!colorfull">metti stile</button>
</div>
</template>

<script>
export default {
    name: 'Test',
    data() {
        return {
            colorfull:false
        }
    }
}
</script>

<style lang="scss">
.green {
    color:blue;
    background-color: green;
}
</style>    