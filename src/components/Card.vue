<script>

</script>

<template>
    <Grid>
        <div>
            <img class="imagen" :src="url"
            :alt="nombre">
            <h2>{{nombre}}</h2>
            <a :href="url"
            target="_blank">
                Descargar
            </a>
        </div>
    </Grid>
</template>

<script>
import Grid from './Grid.vue'
export default ({
    props: {
        url: {
            String,
        },
        enlace: {
            String,
        },
        nombre: {
            String,
        }
    }
})
</script>


<style scoped>
    
    div {
        border: 1px solid #000;
        padding: 2rem;
        border-radius: 2rem;
        margin: 0 auto;
        align-items: center;
        text-align: center;
    }

    .imagen {
        width: 15rem;
        height: 15rem;
    }

    h2 {
        text-align: center;
        text-transform: uppercase;
    }

    a {
        color: #FFF;
        text-decoration: none;
        width: 40%;
        background-color: #301675;
        padding: .75rem;
        border-radius: .3rem;
    }
</style>