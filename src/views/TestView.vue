<template>
  <div>
    <h1>Table view iteration 1</h1>
    <table style="width:100%">
      <tr>
        <th>Firstname</th>
        <th>Lastname</th>
        <th>Age</th>
      </tr>
      <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>50</td>
      </tr>
      <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>94</td>
      </tr>
    </table>
  </div>
  <!--
  <div>
    <table>
      <tr>
        <th v-for="header of headers" :key="header.id">{{ header.text }}</th>
      </tr>
      <tr v-for="node of workflow" :key="node.id">
        <td>{{ node.cyclepoint }}</td>
        <td>{{ node.name }}</td>
        <td>{{ node.state }}</td>...
      </tr>
    </table>
  </div>
  -->

</template>

<script>
// @ = alias to 'src'
// TODO create Comp.vue
// import Comp from '@/components/cylc/comp/Comp.vue'

export default {
  name: 'TestView',
  props: {
    workflowName: {
      type: String,
      required: true
    }
  },

  // components: {
  //   Comp
  // },
  metaInfo () {
    return {
      title: 'Temp View'
    }
  },

  data: () => ({
    workflowTree: {}
  })

}
</script>

<style scoped>

</style>
