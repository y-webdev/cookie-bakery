<template>
    <div class="p-3 overflow-hidden">
        <button class="btn sun rounded-circle float-right" @click="toggleDarkMode"></button>
    </div>
</template>

<script>
const el = document.querySelector('body')
export default {
    methods: {
        toggleDarkMode () {
            el.classList.toggle('bg-dark')
        }
    }
}
</script>

<style scoped>
.sun {
    width: 10rem;
    height: 10rem;
    background: yellow;
}
</style>
