<script>
export default{
    name: "AppHero",
    data() {
        return{
            sfondo: true,
        }
    },
    methods: {
        cambiaSfondo(){
            if(this.sfondo) {
                this.sfondo = false
            } else {
                this.sfondo = true
            }
        }
    },
}
</script>

<template>
    <div>
        <div class="p-5 mb-4 rounded-3" :class="(sfondo)? 'luna': 'sole'">
            <div class="container-fluid py-5">
                <h1 class="text-success">Ciao sono un jumbotron</h1>
                <p class="text-info">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sunt quaerat vel voluptate? Obcaecati commodi vero numquam qui, ea exercitationem quam. Odit obcaecati eum dolorum quas quo eligendi asperiores, ratione quia!</p>
                <button class="btn btn-dark" type="button" @click="cambiaSfondo">Non premermi sono inutile(forse..)</button>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .luna {
        background-image:url(/images/moon.jpg);
    }

    .sole {
        background-image:url(/images/sole.jpeg);
        background-repeat: no-repeat;
        background-size: cover;
        filter: brightness(2);
    }
</style>