<template>
  <div>
    <H1>Hello</H1>
<!--    <comp-->
<!--      :workflows="workflowTree"-->
<!--      ></comp>-->
  </div>
</template>

<script>
// @ = alias to 'src'
// TODO create Comp.vue
// import Comp from '@/components/cylc/comp/Comp.vue'

export default {
  name: "TestWidget",
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