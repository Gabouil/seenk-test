<template>
    <div id="Hobbies" class="main_section">
      <h1>
        💃🏻 HOBBIES
      </h1>
      <p> 
        {{$parent.ourData['hobbies']}}
      </p>  
    </div>
</template>

<script>  

export default {
  name: 'Hobbies'
}
</script>

<style scoped>
p { 
  font-size: 18px;
  line-height: 21px;

  color: #4D4D4D;
}
</style>