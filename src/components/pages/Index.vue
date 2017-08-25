<template>
  <div id="index">
    <my-head></my-head>
    <my-content></my-content>
    <my-foot></my-foot>
  </div>
</template>

<script>
  import Head from '../../components/Head.vue'
  import Foot from '../../components/Foot.vue'
  import Content from '../../components/Content.vue'

  export default {
    name: 'index',
    components: {
      'my-head': Head,
      'my-foot': Foot,
      'my-content': Content
    }
  }
</script>


<style scoped>
  #index{
    background: #f5f5f5;
    /*overflow-y: scroll;*/
  }

</style>
