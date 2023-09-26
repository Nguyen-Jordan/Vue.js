<template>
    
    <h1>{{ meteo.name }}</h1>
    <p>le temp de la météo aujourd'hui: {{ meteo.weather }}</p>
    <p>{{ meteo.temperature }} °C</p>
    <p>{{  meteo.updatedAt.toLocaleString() }}</p>
</template>

<script>
export default {
    data() {
        return {
            meteo: {
                name: 'Annecy', // nom de la ville
                weather: 'Peu nuageux', // descriptif météo 
                temperature: 20.55, // température en °C
                updatedAt: new Date() // date de dernière mise à jour
            }
        }
    }
}
</script>
