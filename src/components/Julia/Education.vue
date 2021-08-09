<template>
    <div id="Education" class="main_section">
      <h1>
        🎓 EDUCATION
      </h1>
      <span>
        <input v-if="$parent.ourData['graduate']" type="checkbox" checked> 
        <input v-else type="checkbox"> 
        <div>
            <h2>Graduate</h2>
            <p>{{$parent.ourData['graduate_comment']}}</p>
        </div> 
      </span>
      <span>
        <input v-if="$parent.ourData['undergraduate']" type="checkbox" checked> 
        <input v-else type="checkbox"> 
        <div>
          <h2>Undergraduate</h2>
            <p>{{$parent.ourData['undergraduate_comment']}}</p>
        </div>
      </span>
      <span>
        <input v-if="$parent.ourData['highschool']" type="checkbox" checked> 
        <input v-else type="checkbox"> 
        <div>
          <h2>High school</h2>
            <p>{{$parent.ourData['highschool_comment']}}</p>
        </div>
      </span>
    </div>
</template>

<script>

export default {
  name: 'Education'
}
</script>

<style scoped>

span div{
  display: flex;
  flex-direction: column;
}
span {
  display: flex;
  margin-bottom: 10px;
}
input {
  align-self: flex-start;
  margin-right: 10px;
}
h2 {
  margin-bottom: 5px;
  font-size: 15px;
}
p {
  font-size: 12px;
  color: #818181;
}
</style>