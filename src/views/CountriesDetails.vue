<template>
    
    {{$route.params.code}}
    <div v-for="(country, index) in countries">
    <div class="column is-8">
        <section class="section">
            <figure class="image is-128x128">
                <img/>
            </figure>
            <div class="title">France</div>
            <table class="table is-fullwidth">
                <tbody>
                    <tr>
                        <td>Capital</td>
                        <td>Paris</td>
                    </tr>
                    <tr>
                        <td>Area</td>
                        <td>551695 km <sup>2</sup></td>
                    </tr>
                    <tr>
                        <td>Borders</td>
                        <td>
                            <ul>
                                <li><a href="/AND">Andorra</a></li>
                                <li><a href="/BEL">Belgium</a></li>
                                <li><a href="/DEU">Germany</a></li>
                                <li><a href="/ITA">Italy</a></li>
                                <li><a href="/MCO">Monaco</a></li>
                                <li><a href="/ESP">Spain</a></li>
                                <li><a href="/CHE">Switzerland</a></li>
                            </ul>
                        </td>
                    </tr>
                </tbody>
            </table>
        </section>
    </div>
</div>

</template>

<script setup>
import countriesData from '../assets/countries.json'
import { useRoute, useRouter } from 'vue-router'

const route = useRoute(); 
const router = useRouter(); 


</script>

<style scoped>

</style>

