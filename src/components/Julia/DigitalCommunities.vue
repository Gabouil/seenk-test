<template>
    <div id="DigitalCommunities" class="main_section">
      <h1>📱 DIGITAL COMMUNITIES</h1>
      <div class="logo_container">
        <img :src="logo" alt="" v-for="logo in $parent.ourData['communities']" :key="logo">
      </div>
    </div>
</template>

<script>
export default {
  name: 'DigitalCommunities'
}
</script>

<style scoped>
img {
  height: 52px;
  width: 52px;
  margin: 0 5px 0 5px;
}
.logo_container {
  width: 60%;
  display: flex;
  justify-content: space-between;
}
</style>
