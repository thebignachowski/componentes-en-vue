import { default } from '../App.vue';
<template>
    <div class="componente">
        <div class="logo">
            <img src="../assets/logo.svg" alt="logo aplicación">
        </div>
        <div class="title">
            <h1>{{title}}</h1>
        </div>
    </div>
</template>

<script>
    export default ({
        props: {
            title: {
                String,
            }
        }
    })
</script>

<style scoped>
.componente {
    min-height: 5rem;
    background-color: #ACA51D;
    display: flex;
    flex-direction: column;
    align-items: center;
}

@media (min-width: 768px) {
    .componente {
        display: flex;
        flex-direction: row;
        justify-content: space-around;
    }
}

.logo img{
    width: 4rem;
    height: 4rem;
}

.title h1 {
    color: #FFF;
    text-align: center;
    text-transform: uppercase;
}
</style>