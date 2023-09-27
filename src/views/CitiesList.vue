<template>
    <div class="citiesList">
        <h1>Météo - Liste des villes</h1>
        <city v-for="city in cities" :key="city.id" :name="city.name" :weather="city.weather" :temperature="city.temperature" :updated-at="city.updatedAt. toLocaleString()"/>
    </div>
</template>

<script>
import City from "../components/City.vue"

export default {
    data() {
        return {
            cities: [
                {
                    id: 1,
                    name: 'Madrid',
                    weather: 'Ensoleillé',
                    temperature: 42.0,
                    updatedAt: new Date()
                },
                {
                    id: 2,
                    name: 'Paris',
                    weather: 'Peu nuageux',
                    temperature: 19.5,
                    updatedAt: new Date()
                }
            ]
        }
    },
    components: {
        City
    }
}
</script>

<style>
h1{
    color: #BCEBFA;
    text-align: center;
    margin-bottom: 22px;
}

h2{
    padding-bottom: 12px;
    text-align: center;
    color: #72ADD1;
    font-weight: bold;
}
span{
    color: white;
}
p{
    text-align: center;
    margin: 0 15px 0 15px;
}
.ville-bloc{
    display: flex;
    flex-direction: column;
    margin: 15px 0 15px 0;
}
.ville-content{
    display: flex;
    flex-direction: row;

}
</style>
  
  