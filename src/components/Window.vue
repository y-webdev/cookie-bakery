<template>
    <div class="window rounded-circle mx-auto mt-5">
        <img src="../assets/cookie.png" class="w-100" alt="Cookie">
    </div>
</template>

<script>
export default {}
</script>

<style scoped>
.window {
    width: 8rem;
    height: 8rem;
    background: lightblue;
    border: .2rem solid cornflowerblue;
    cursor: pointer;
}

.window img {
    display:none;
}

.window:hover {
    background: #643212;
    border: .2rem solid #643212;
}

.window:hover img {
    display:block;
}

.bg-dark .window:hover {
    background: lightblue;
    border: .2rem solid cornflowerblue;
}

.bg-dark .window:hover img {
    display:none
}
</style>
