<template>
  <table style="width:100%">
    <tr style="text-align: left">
      <th>task</th>
      <th>state</th>
      <th>host</th>
      <th>job system</th>
      <th>job ID</th>
      <th>T-submit</th>
      <th>T-start</th>
      <th>T-finish</th>
      <th>dT-mean</th>
      <th>latest message</th>
    </tr>
    <tr>
      <td>Jill</td>
      <td>Smith</td>
      <td>50</td>
      <td>Jill</td>
      <td>Smith</td>
      <td>50</td>
      <td>Jill</td>
      <td>Smith</td>
      <td>50</td>
      <td>50</td>
    </tr>
    <tr>
      <td>Eve</td>
      <td>Jackson</td>
      <td>94</td>
      <td>Eve</td>
      <td>Jackson</td>
      <td>94</td>
      <td>Eve</td>
      <td>Jackson</td>
      <td>94</td>
      <td>94</td>
    </tr>
  </table>

</template>

<script>
export default {
  name: "TableView"
}
</script>

<style scoped>

</style>