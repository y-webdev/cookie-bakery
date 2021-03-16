<template>
    <button class="btn h-75 w-100 position-absolute"></button>
</template>

<script>
export default {}
</script>

<style scoped>
button {
    bottom:0;
    left:0;
    background: lightsalmon;
}
button:after {
    content:"";
    position:absolute;
    top:50%;
    left:2rem;
    transform: translateX(-50%);
    width: 3.25rem;
    height: .75rem;
    background: saddlebrown;
    border-radius: .25rem;
}
</style>
