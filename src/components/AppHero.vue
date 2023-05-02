<script>
export default{
    name: "AppHero",
    data() {
        return{
            luna: "'/images/moon.jpg'",



        }
    }
}
</script>

<template>
    <div>
        <div class="p-5 mb-4 rounded-3" id="jumbo">
            <div class="container-fluid py-5">
                <h1 class="text-success">Ciao sono un jumbotron</h1>
                <p class="text-info">forse...</p>
                <button class="btn btn-dark" type="button">Non premermi sono inutile</button>
            </div>
        </div>
    </div>
</template>

<style scoped>
    #jumbo {
        background-image:url(/images/moon.jpg);
    }
</style>