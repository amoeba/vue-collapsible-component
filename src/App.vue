<template>
  <div id="app">
    <CollapsiblePane>
      <PaneOne />
    </CollapsiblePane>
    <CollapsiblePane>
      <PaneTwo />
    </CollapsiblePane>
  </div>
</template>

<script>
import CollapsiblePane from './components/CollapsiblePane.vue'
import PaneOne from './components/PaneOne.vue'
import PaneTwo from './components/PaneTwo.vue'

export default {
  name: 'app',
  components: {
    CollapsiblePane,
    PaneOne,
    PaneTwo
  }
}
</script>

<style>
#app {
  font-family: sans-serif;
}
.title {
  cursor: pointer;
}
</style>
