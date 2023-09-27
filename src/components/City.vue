<template>
    <div class="ville-bloc">
        <h2>{{ name }}</h2>
        <div class="ville-content">
            <p class="weather">temp <br><span>{{ weather }}</span></p><br>
            <p class="temp">La température moyenne<br> <span>{{ temperature }} °C</span></p>
            <p class="date">La dernière actualisation:<br><span>{{ updatedAt }}</span></p>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {

        }
    },
    props: { name: String, weather: String, temperature: Number, updatedAt: Date }
}
</script>
