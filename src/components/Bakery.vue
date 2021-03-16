<template>
    <div class="wrapper m-auto mt-3">
        <Sun/>
        <Roof/>
        <b-row class="mx-1 position-relative">
            <Plate/>
            <b-col>
                <Window/>
            </b-col>
            <b-col class="position-relative">
                <Door/>
            </b-col>
            <b-col class="position-relative">
                <Window/>
                <Mailbox/>
            </b-col>
        </b-row>
    </div>
</template>

<script>
    import Sun from '@/components/Sun'
    import Roof from '@/components/Roof'
    import Plate from '@/components/Plate'
    import Window from '@/components/Window'
    import Door from '@/components/Door'
    import Mailbox from '@/components/Mailbox'

    export default {
        components: {
            Sun,
            Roof,
            Plate,
            Window,
            Door,
            Mailbox
        }
    }
</script>

<style scoped>
.wrapper {
    width: 33rem;
    margin: 1rem;
}

.row {
    height: 25rem;
    background: darkgray;
}
</style>
