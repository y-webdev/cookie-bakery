<template>
  <div id="app">
    <Bakery/>
  </div>
</template>

<script>
import Bakery from "@/components/Bakery";

export default {
  name: 'App',
  components: {
    Bakery
  }
}
</script>

<style>
.bg-dark * {
    opacity: .9;
}
</style>
