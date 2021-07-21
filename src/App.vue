<template>
    <div id="app">
        <CustomTitle :titleText="message" :subtitleText="subMessage"/>
        <img  class="poke" src="./assets/pokedex.png" alt="">
        <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
        <Pokemons />
    </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
import CustomTitle from "./components/CustomTitle.vue";
import Pokemons from "./pages/Pokemons.vue";

export default {
    name: "App",
    components: {
        // HelloWorld
        CustomTitle,
        Pokemons,
    },
    data() {
        return {
            message: "Pokedex",
            subMessage: "Giochiamo con i Pokemon"
        }
    }
};
</script>

<style lang="scss">
@import './assets/scss/app.scss';
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
    .poke {
        width: 300px;
        margin: 20px 0;
    }
}
</style>
