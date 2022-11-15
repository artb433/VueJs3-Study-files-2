<template>
   <div class="container">
    <div class="row">
      <div class="col">
        <p class="h3">Employee</p>
        <ul class="list-group">
          <li class="list-group-item">
            Name: {{employee.name}}
          </li>
          <li class="list-group-item">
            Age: {{employee.age}}
          </li>
          <li class="list-group-item">
            Designation: {{employee.designation}}
          </li>
          
        </ul>
      </div>
    </div>
   </div>
</template>

<script>
export default {
  name: "Employee",
data: function() {
    return {
      //maintain state
      employee: {
        name: 'Rajan',
        age: 26,
        designation: 'Software Engineer'
      }
    }
},
};
</script>

<style lang="scss" scoped></style>