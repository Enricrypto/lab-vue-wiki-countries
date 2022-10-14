<template>
    <div v-for="(country, index) in countries" class="column is-4" style="overflow: auto">
        <router-link :to="{name:'details', params:{code:country.alpha3Code}}">
            <a class="media is-clickable name-map" href=":code">
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
<router-view></router-view> 
</template>

<script setup>
import countries from '../assets/countries.json'
import { useRoute }  from 'vue-router'

const route = useRoute();

</script>

<style scoped>
.name-map {
    display: flex; 
    flex-direction: column;
    justify-content: center; 
    align-items: center;
    text-align: center; 
    margin: 0px;
    padding: 0px; 

}

.content p {
    text-decoration: none; 
    color: black
}

.media {
}

</style>

