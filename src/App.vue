
<script setup>
import { ref } from 'vue';

const inputText = ref('hello')
const grade = ref('')

</script>
<template>
  <div  >
  <div class="mx-auto p-2" style="width: 400px; " >
    
  <div class="p-3 mb-2 bg-dark-subtle text-emphasis-dark">
    <h1>View Grade</h1>
    
    <select v-model="grade"  class="form-select form-select-lg mb-3" aria-label="Large select example">
        <option value="math">Math</option>
        <option value="english">English</option>
        <option value="filipino">Filipino</option>
        <option value="science">Science</option>
        <option value="mapeh">Mapeh</option> 
        <option value="esp">ESP</option> 
        <option value="aralpan">Araling Panlipunan</option>
        
        
        
       
    </select>
    <p v-if="grade == 'math'">
    <h1>87</h1>
    </p>
    <p v-if="grade == 'english'">
      <h1></h1>
  </p>
  <p v-if="grade == 'filipino'">
    <h1>88</h1>
  </p>
  <p v-if="grade == 'science'">
    <h1>98</h1>
  </p>
  <p v-if="grade == 'mapeh'">
    <h1>84</h1>
  </p>
  <p v-if="grade == 'esp'">
    <h1>90</h1>
  </p>
  <p v-if="grade == 'aralpan'">
    <h1>93</h1>
  </p>
</div>
</div>
</div>

</template>