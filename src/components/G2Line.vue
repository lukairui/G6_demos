<template>
  <div id="mountNode"></div>
</template>

<script>
import G6 from '@antv/g6'
let data = {
  nodes: [{
    id: 'node1',
    x: 100,
    y: 200
  },
  {
    id: 'node2',
    x: 300,
    y: 200
  }],
  edges: [{
    source: 'node1',
    target: 'node2'
  }]
}
let graph = new G6.Graph({
  container: 'mountNode',
  width: 500,
  height: 500
})
graph.data(data)
graph.render()
export default {
  data () {
    return {
      chart: 'test'
    }
  }
}
</script>
