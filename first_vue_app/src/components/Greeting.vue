<template>
  <div class="container">
    <div class="row">
      <div class="col-md-5 ">
        <div class="card shadow-lg">
          <div class="card-body">
            <p class="h3 display-3">Hello,<span class="fw-bold">{{this.msg}}</span></p>
            <button class="btn btn-success m-1" @click="greet(value='Good Morning')">Good Morning</button>
            <button class="btn btn-warning m-1" @click="greet(value='Good Afternoon')">Good Afternoon</button>
            <button class="btn btn-danger m-1" @click="greet(value='Good Evening')">Good Evening</button>
            
            <!-- //Alternatively
            <button class="btn btn-success m-1" @click="msg='Good Morning'">Good Morning</button>
            <button class="btn btn-warning m-1"  @click="msg='Good Afternoon'">Good Afternoon</button>
            <button class="btn btn-danger m-1"  @click="msg='Good Evening'">Good Evening</button> -->
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Greeting",
  created() {},
  data() {
    return {
      msg:""
    };
  },
  props: {},
  methods: {
    greet(value) {
      this.msg = value;
  },
}
};
</script>

<style lang="scss" scoped></style>