<template>
  <canvas id="canvas_2"></canvas>
</template>

<script>
import 'fabric';

export default {
  name: 'CanvasNotWorking',
  data() {
    return {
      canvas2: null
    }
  },
  async mounted() {
    this.canvas2 = new fabric.Canvas('canvas_2', {
      width: 400,
      height: 200,
    });

    this.canvas2.add(new fabric.Polygon([{x: 0, y: 0}, {x: 100, y: 100}, {x: 200, y: 100}]))
    this.canvas2.add(new fabric.Polygon([{x: 200, y: 110}, {x: 250, y: 160}, {x: 270, y: 110}]))
  },
}
</script>
