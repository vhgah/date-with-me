<template>
  <canvas
    ref="canvas"
    id="fabric-canvas"
    class="basis-7/12 border"
    width="800"
    height="1000"
  ></canvas>
</template>

<script>
import * as fabric from 'fabric'
export default {
  mounted() {
    // Initialize Fabric.js canvas
    this.canvas = new fabric.Canvas(this.$refs.canvas)

    // Set canvas background color
    this.canvas.backgroundColor = '#292929'

    // Render wedding timeline
    this.renderTimeline()
  },
  methods: {
    renderTimeline() {
      // Title text
      var titleText = new fabric.IText('Wedding Timeline', {
        left: this.canvas.width / 2,
        top: 20,
        fontSize: 30,
        fill: 'white',
        fontWeight: 'bold',
        originX: 'center'
      })
      this.canvas.add(titleText)

      // Event 1
      var event1Group = new fabric.Group(
        [
          new fabric.IText('11:30 AM', {
            fontSize: 18,
            fontWeight: 'bold',
            fill: 'white',
            originX: 'right'
          }),
          new fabric.IText('Wedding Ceremony', {
            fontSize: 14,
            fill: '#ccc',
            top: 30,
            originX: 'right'
          })
        ],
        {
          left: 20,
          top: 100,
          originX: 'left',
          originY: 'top'
        }
      )

      this.canvas.add(event1Group)

      // Event 2
      var event2Group = new fabric.Group(
        [
          new fabric.IText('1:00 PM', {
            fontSize: 18,
            fontWeight: 'bold',
            fill: 'white',
            originX: 'right'
          }),
          new fabric.IText('Wedding lunch', {
            fontSize: 14,
            fill: '#ccc',
            top: 30,
            originX: 'right'
          })
        ],
        {
          left: 20,
          top: 250,
          originX: 'left',
          originY: 'top'
        }
      )

      this.canvas.add(event2Group)

      // Render canvas
      this.canvas.renderAll()
    }
  }
}
</script>
