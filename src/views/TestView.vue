<template>
  <div>
    <h1>Table view iteration 1</h1>
  </div>
  <div>
    <table>
      <tr>
        <th v-for="header of headers" :key="header.id">{{ header.text }}</th>
      </tr>
      <tr v-for="node of workflow" :key="node.id">
        <td>{{ node.cyclepoint }}</td>
        <td>{{ node.name }}</td>
        <td>{{ node.state }}</td>
        <!-- ...
        -->
      </tr>
    </table>
  </div>
</template>

<script>
// @ = alias to 'src'
// TODO create Comp.vue
// import Comp from '@/components/cylc/comp/Comp.vue'

export default {
  name: "TestView",
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