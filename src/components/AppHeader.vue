<template>
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <div class="container-fluid">
            <a class="navbar-brand" href="#">Navbar</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                    <li class="nav-item">
                        <router-link class="nav-link"
                        :class="this.$route.name === 'home' ? 'active': ''"
                        aria-current="page" :to="{name: 'home'}">
                            Home
                        </router-link>
                    </li>
                    <li class="nav-item">
                        <router-link class="nav-link"
                        :class="this.$route.name === 'projects' ? 'active': ''"
                        :to="{ name: 'projects'}">
                            Projects
                        </router-link>
                    </li>
                    <li class="nav-item">
                        <router-link class="nav-link"
                        :class="this.$route.name === 'about' ? 'active': ''"
                        :to="{ name: 'about'}">
                            About us
                        </router-link>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>

</style>