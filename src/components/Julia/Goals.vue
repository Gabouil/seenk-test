<template>
    <div id="Goals" class="main_section">
      <h1>
        🎯 GOALS
      </h1>
      <p>
        {{$parent.ourData['goals']}}
      </p>
    </div>
</template>

<script>

export default {
  name: 'Goals'
}
</script>

<style scoped>
p {
  line-height: 21px;
}
</style>