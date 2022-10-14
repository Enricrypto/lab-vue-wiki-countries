<template>
    <nav class="navbar" role="navigation" aria-label="main navigation">
        <div class="navbar-brand">
            <a class="navbar-item">
                <router-link class="navbar-item has-text-weight-semibold" :to="{name: 'countries'}">LAB -
                    WikiCountries</router-link>
            </a>

        </div>
    </nav>
</template>

<script setup>

</script>

<style scoped>
.navbar-item{
    background-color: blue;
    color: white;
    width: 100%;
}

.navbar {
    position: sticky; 
    top: 0px; 
}
</style>