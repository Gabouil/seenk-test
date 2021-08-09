<template>
  <mainPageJulia />
  <mainPageGreg />
</template>

<script>
import mainPageJulia from './view/mainPageJulia.vue'
import mainPageGreg from './view/mainPageGreg.vue'

export default {
  name: 'App',
  components: {
    mainPageJulia,
    mainPageGreg
  }
}
</script>


<style src="./reset.css"></style>
<style>
@font-face {
 font-family: "SFProText";
 src: url("./fonts/SFProText-Regular.ttf");
}
body {
  font-family: "SFProText";
  color: #4D4D4D;
  font-size: 15px;
}
</style>
