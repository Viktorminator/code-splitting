<template>
  <div id="app">
    <button @click="show=true">Load tooltip</button>
    <div v-if="show">
      <Tooltip/>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({ show: false }),
  components: {
    Tooltip: () => import("@/components/Tooltip")
  }
}
</script>