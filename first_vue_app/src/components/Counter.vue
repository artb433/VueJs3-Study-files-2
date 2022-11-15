<template>
  <div class="container">
    <div class="row">
      <div class="col-md-4">
        <div class="card shadow-lg">
          <div class="card-body">
            <p class="h3 display-3">{{this.count}}</p>
            <button @click="this.incr()" class="btn btn-success m-1">Increment</button>
            <button @click="this.decr()" class="btn btn-warning m-1">Decrement</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Counter",
  created() {},
  data() {
    return {
      count: 0
    };
  },
  // props: {},
  methods: {
    incr(){
      this.count=this.count + 1
    },
    decr(){
      if (this.count!=0) {
        this.count=this.count - 1
      } else {
        this.count=this.count
      }

    }
  },
};
</script>

<style lang="scss" scoped></style>