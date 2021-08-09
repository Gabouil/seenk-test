<template>
    <div id="Frustrations" class="main_section">
      <h1>
        😈 FRUSTRATIONS
      </h1>
      <p>
        {{$parent.ourData['frustration']}}
      </p>
    </div>
</template>

<script>

export default {
  name: 'Frustrations'
}
</script>

<style scoped>
p {  
  line-height: 21px;
}
</style>