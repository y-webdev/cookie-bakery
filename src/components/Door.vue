<template>
    <button class="btn h-75 w-100 position-absolute" @click="saveKnock"></button>
</template>

<script>
export default {
    data () {
        return {
            time: {
                click: Date.now()
            }
        }
    },
    methods: {
        async saveKnock () {
            try {
                const response = await fetch('http://localhost:3000/clicks', {
                    method: 'POST',
                    headers: {
                        'Content-Type': 'application/json'
                    },
                    body: JSON.stringify(this.time)
                })
                return response.json()
            } catch (err) {
                throw new Error('Something went wrong.')
            }
        }
    }
}
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
