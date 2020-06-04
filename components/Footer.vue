<template>
  <div class="layout-bottom">
    <div class="container has-text-centered">
      <p>Marcadores: {{ sheetData.rows.length }}</p>
    </div>
  </div>
</template>

<script>
export default {
  computed: {
    sheetData () {
      return this.$store.state.sheet.data
    }
  }
}
</script>

<style lang="scss" scoped>
.layout-bottom {
  background-color: $primary;
  padding: 3px;
  font-size: 0.8rem;
  color: #fff;
  order: 0;
  flex: 0 1 auto;
  align-self: auto;
  border-top: 1px solid #FFF;
}
</style>
