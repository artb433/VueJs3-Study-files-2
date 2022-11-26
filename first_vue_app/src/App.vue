<template>
 <div class="container mt-3">
  <div class="grid">
   <div class="row">
    <div class="col">
     <p class="h3 text-success fw-bold">
      App Component
     </p>
     <p class="fw-bold fs-5">Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas nisi architecto repellendus blanditiis in magnam laudantium ut saepe harum sit, natus illum minima doloremque amet perspiciatis asperiores praesentium molestias velit!</p>
    </div>
   </div>
  </div>

  <!-- <Customer name="Rajan" age="25" /> -->
  <Employee/>
  <Counter/>
  <Greeting/>
  <Register/> 
  <Customer/>

  
 </div>
 
</template>

<script>  
import Counter from './components/Counter.vue';
import Customer from './components/Customer.vue';
import Employee from './components/Employee.vue';
import Greeting from './components/Greeting.vue';
import Register from './components/Register.vue';

export default {
    components: {
    Customer,
    Employee,
    Counter,
    Greeting,
    Register
}
}



</script>

<style>
 @import "./style.css";
</style>
