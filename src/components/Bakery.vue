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
    import Sun from './Sun'
    import Roof from './Roof'
    import Plate from './Plate'
    import Window from './Window'
    import Door from './Door'
    import Mailbox from './Mailbox'

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
