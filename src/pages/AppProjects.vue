<template>
    <div class="container">
        <div class="row">
            <SingleCard v-for="project in projects" 
            :title = "project.title"
            :description = "project.description"/>
        </div>
    </div>
</template>

<script>
    import axios from 'axios';
    import SingleCard from '../components/SingleCard.vue';

    export default {
        name: "AppProjects",
        data() {
        return {
            projects : []
        }
        },
        mounted () {
        axios
        .get('http://127.0.0.1:8000/api/projects')
        .then((response) => {
            this.projects = response.data.results;
            console.log(this.projects);
        })
        },
        components : {
        SingleCard
        }
    }
</script>

<style lang="scss" scoped>

</style>