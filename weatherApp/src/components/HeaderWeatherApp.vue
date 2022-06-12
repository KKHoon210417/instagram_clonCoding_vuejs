<template>
    <div class="headerContainer">
        <div class="location">{{ propsdata.location }}</div>
        <div class="title">{{ propsdata.currentTemp }}</div>
        <div class="description">{{ propsdata.weatherDesc }}</div>
        <div class="mini-description">최고: {{ propsdata.maxTemp }} 최저: {{ propsdata.minTemp }}</div>
    </div>
</template>

<script>
export default {
    props: ['propsdata']

}
</script>

<style scoped>
.headerContainer .title {
    font-size: 100px;
}

.headerContainer .location {
    font-size: 50px;
    margin-bottom: 5px;
    margin-top: 2.5rem;
}

.headerContainer .description {
    font-size: 30px;
}

.headerContainer .mini-description {
    font-size: 20px;
}


.headerContainer {
    margin-top: 100px;
}

</style>
