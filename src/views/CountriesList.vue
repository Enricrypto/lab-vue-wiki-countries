<template>
    <div v-for="(country, index) in countries" class="column is-4" style="overflow: auto">
        <router-link :to="{name:'countries', params:{code:index}}">
            <a class="media is-clickable" href="/1">
                <figure class="media-left">
                    <p class="image is-64x64">
                        <img
                            :src="`https://flagpedia.net/data/flags/icon/72x54/${country.alpha2Code.toLowerCase()}.png`" />
                    </p>
                </figure>
                <div class="media-content">
                    <div class="content">
                        <p>
                            <strong>{{country.name.common}}</strong>
                        </p>
                    </div>
                </div>
            </a>
        </router-link>
    </div>

<router-view/>
</template>

<script setup>
import countries from '../assets/countries.json'

console.log(countries)

</script>

<style scoped>

</style>

