<template>
  <div
    class="d-flex card"
    :style="{
      'grid-column-start': XStart || 'auto',
      'grid-column-end': XEnd || 'auto',
      'grid-row-start': YStart || 'auto',
      'grid-row-end': YEnd || 'auto'
    }">
    <component class="card-content" :is="currentComponent"/>
  </div>
</template>

<script>

import Header from './Header.vue'

export default {
  name: 'CharSheetMain',
  components: {
    Header
  },
  props: {
    XStart: [String, Number],
    XEnd: [String, Number],
    YStart: [String, Number],
    YEnd: [String, Number],
    currentComponent: {
      type: String,
      default: 'div'
    }
  },
  data () {
    return {
    }
  },
  methods: {
  }
}
</script>

<style scoped lang="scss">
.card {
  padding: .5em;
}

.card-content {
  border: 2px solid black;
  width: 100%;
  border-radius: 1em;
}
</style>
