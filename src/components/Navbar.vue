<template>
    <div>
        <nav class="navbar is-info" role="navigation" aria-label="main navigation">
            <div class="container">
                <div class="navbar">
                    <router-link class="navbar-item has-text-weight-semibold" :to="{name:'countries'}">
                        {{navbarName()}}
                    </router-link>
                </div>
            </div>
        </nav>
    </div>
</template>

<script setup>
const navbarName = () => {
    return `LAB - WikiCountries`;
}
</script>

<style scoped>

</style>