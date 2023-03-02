<template>
  <div>
    <ul>
      <li v-for="project in projects" :key="project.id">
        {{ project }}
      </li>
    </ul>
  </div>
</template>

<script>
  import axios from 'axios';
  export default {
    data() {
      return {
        projects : []
      }
    },
    methods: {
      name() {
        
      }
    },
    mounted () {
    axios
      .get('http://127.0.0.1:8000/api/projects')
      .then((response) => {
        this.projects = response.data.results;
        console.log(this.projects);
      })
    }
  }
</script>

<style lang="scss" scoped>

</style>
