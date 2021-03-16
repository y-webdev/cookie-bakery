<template>
    <div class="mailbox h-25 bg-secondary mt-5 pt-2" @click="toggleActive" :class="{ active: isActive }">
        <div class="p-2 mx-3 mt-2 bg-dark"></div>
        <p class="text-center h5 mt-2">Mailbox</p>
    </div>
</template>

<script>
export default {
    data () {
        return {
            isActive: false
        }
    },
    methods: {
        toggleActive () {
            this.isActive = !this.isActive
        }
    }
}
</script>

<style scoped>
.mailbox {
    cursor:pointer;
}

.mailbox.active {
    position: absolute;
    bottom: 0;
    width: calc(100% - 30px);
    animation: shake 0.5s;
    animation-iteration-count: 1;
}

@keyframes shake {
    0% { transform: translate(1px, 1px) rotate(0deg); }
    10% { transform: translate(-1px, -2px) rotate(-1deg); }
    20% { transform: translate(-3px, 0px) rotate(1deg); }
    30% { transform: translate(3px, 2px) rotate(0deg); }
    40% { transform: translate(1px, -1px) rotate(1deg); }
    50% { transform: translate(-1px, 2px) rotate(-1deg); }
    60% { transform: translate(-3px, 1px) rotate(0deg); }
    70% { transform: translate(3px, 1px) rotate(-1deg); }
    80% { transform: translate(-1px, -1px) rotate(1deg); }
    90% { transform: translate(1px, 2px) rotate(0deg); }
    100% { transform: translate(1px, -2px) rotate(-1deg); }
}
</style>
