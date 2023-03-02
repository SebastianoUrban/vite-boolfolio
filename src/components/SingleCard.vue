<template>
  <div class="col-4">
    <div class="card mt-4">
      <div class="card-body">
        <div class="card-title">
          <h2 class="">{{ title }}</h2>
        </div>
        <div class="card-text">
          <h5>Description:</h5>
          <p class="">{{ description }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
      }
    },
    methods: {
    },
    props : {
      title : String,
      description : String
    }
  }
</script>

<style lang="scss" scoped>

</style>