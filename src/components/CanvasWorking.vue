<template>
  <canvas id="canvas_3"></canvas>
</template>

<script>
import 'fabric';

export default {
  name: 'CanvasWorking',
  async mounted() {
    const canvas = new fabric.Canvas('canvas_3', {
      width: 400,
      height: 200,
    });

    canvas.add(new fabric.Polygon([{x: 0, y: 0}, {x: 100, y: 100}, {x: 200, y: 100}]))
    canvas.add(new fabric.Polygon([{x: 200, y: 110}, {x: 250, y: 160}, {x: 270, y: 110}]))
  },
}
</script>
