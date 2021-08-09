<template>
    <div id="Education" class="main_section">
      <h1>
        🎓 EDUCATION
      </h1>
      <span>
        <input type="checkbox" checked>
        <div>
            <h2>Graduate</h2>
            <p>Did his Masters in Digital Media at HES</p>
        </div> 
      </span>
      <span>
        <input type="checkbox" checked> 
        <div>
          <h2>Undergraduate</h2>
          <p>Went to a state college, but took generic mid-level courses. </p>
        </div>
      </span>
      <span>
        <input type="checkbox" checked>
        <div>
          <h2>High school</h2>
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