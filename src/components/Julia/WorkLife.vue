<template>
    <div id="WorkLife" class="main_section">
        <h1>
          💼 WORK LIFE
        </h1>
        <div>
          <h2 v-for="tag in $parent.ourData['tags']" :key="tag">{{tag}}</h2>
        </div>
        <p>
          {{$parent.ourData['worklife']}}
        </p>
    </div>
</template>

<script>

export default {
  name: 'WorkLife'
}
</script>

<style scoped>
.main_section div {
  display: flex;
  margin-bottom: 10px;
}
h2 {
  background-color: #F4F4F4;
  border-radius: 3px;
  padding: 2px 9px 2px 9px;
  color: #4B6A87;
  font-size: 14px;
  margin-right: 10px;
}
</style>