<template>
  <div>
    <comp
        :workflows="table"
    ></comp>
  </div>
</template>

<script>
import TableComponent from '@/components/cylc/Table.vue'
export default {
  name: "Table"
}
</script>

<style scoped>

</style>
