<template>
  <div class="bubble-maps-page">
    <div class="row">
      <div class="col-md-12">
        <vuestic-widget class="widget-viewport-height" headerText="Line Maps">
          <line-map v-bind:map-data="lineMapData"></line-map>
        </vuestic-widget>
      </div>
    </div>
  </div>
</template>

<script>
  import LineMap from './LineMap'
  import LineMapData from 'data/maps/LineMapData'

  export default {
    name: 'line-maps-page',
    components: {
      LineMap
    },
    data: function () {
      return {
        lineMapData: LineMapData
      }
    }
  }
</script>

<style lang="scss">

</style>
