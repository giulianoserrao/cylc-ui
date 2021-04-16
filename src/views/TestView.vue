<template>
  <div>
    <h1>Table view iteration 5</h1>
    <table width="100%">
      <tr>
        <th style="text-align: left">task</th>
        <th style="text-align: left">state</th>
        <th style="text-align: left">host</th>
        <th style="text-align: left">job system</th>
        <th style="text-align: left">job ID</th>
        <th style="text-align: left">T-submit</th>
        <th style="text-align: left">T-start</th>
        <th style="text-align: left">T-finish</th>
        <th style="text-align: left">dT-mean</th>
        <th style="text-align: left">latest message</th>
      </tr>
      <tr>
        <td>The</td>
        <td>Smiths</td>
        <td>95</td>
      </tr>
      <tr>
        <td>Queen</td>
        <td>-</td>
        <td>94</td>
      </tr>
      <tr>
        <td>Guns</td>
        <td>'n Roses</td>
        <td>86</td>
      </tr>
      <tr>
        <td>Red Hot</td>
        <td>Chilli Peppers</td>
        <td>73</td>
      </tr>
      <tr>
        <td>The</td>
        <td>Strokes</td>
        <td>84</td>
      </tr>
      <tr>
        <td>Blink</td>
        <td>182</td>
        <td>83</td>
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
