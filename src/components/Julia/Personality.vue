<template>
    <div id="Personality" class="main_section">
      <h1>
        🎭 PERSONALITY
      </h1>
      <p>{{$parent.ourData['personality'][0]}}</p>
      <p>{{$parent.ourData['personality'][1]}}</p>
    </div>
</template>

<script>

export default {
  name: 'Personality'
}
</script>

<style scoped>
.main_section p {
  font-size: 12px;
  color: #C4C4C4;
}
.main_section p:last-child {
  font-size: 18px;
  color: black;
}
</style>