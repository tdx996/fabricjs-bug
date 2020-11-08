<template>
  <h2>Working</h2>
  <p>
    Not assigning canvas to data property.
  </p>
  <canvas-working/>

  <h2>Not working</h2>
  <p>
    Assigning canvas to data property.
  </p>
  <canvas-not-working/>
</template>

<style>
canvas {
  border: 1px solid;
}
</style>

<script>
import 'fabric';
import CanvasNotWorking from "./components/CanvasNotWorking.vue";
import CanvasWorking from "./components/CanvasWorking.vue";

export default {
  name: 'App',
  components: {CanvasWorking, CanvasNotWorking},
}
</script>
