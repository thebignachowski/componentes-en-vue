<template>
  <Header title="Componentes"></Header>

  <div class="contenedor">
    <Card 
      url="https://cdn.svgporn.com/logos/vue.svg?response-content-disposition=attachment%3Bfilename%3Dvue.svg"
      nombre="Vue js"></Card>
    <Card 
      url="https://cdn.svgporn.com/logos/python.svg?response-content-disposition=attachment%3Bfilename%3Dpython.svg"
      nombre="Python"></Card>
    <Card 
      url="https://cdn.svgporn.com/logos/react.svg?response-content-disposition=attachment%3Bfilename%3Dreact.svg"
      nombre="React js"></Card>
    <Card 
      url="https://cdn.svgporn.com/logos/angular-icon.svg?response-content-disposition=attachment%3Bfilename%3Dangular-icon.svg"
      nombre="Angular"></Card>
    <Card
      url="https://cdn.svgporn.com/logos/goland.svg?response-content-disposition=attachment%3Bfilename%3Dgoland.svg"
      nombre="Go"></Card>
    <Card
      url="https://cdn.svgporn.com/logos/javascript.svg?response-content-disposition=attachment%3Bfilename%3Djavascript.svg"
      nombre="Javascript"></Card>
    <Card
      url="https://cdn.svgporn.com/logos/goland.svg?response-content-disposition=attachment%3Bfilename%3Dgoland.svg"
      nombre="Go"></Card>
  </div>
</template>

<style scoped>
h1 {
  border-bottom: 1px solid #000;
  padding-bottom: 1rem;
  text-align: center;
  font-size: 2.4rem;
}

.contenedor {
  width: 90%;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  gap: 1rem;
  margin-top: 2rem;
}


@media (min-width: 768px) {
  .contenedor {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
  }
  h1 {
    font-size: 4rem;
  }
}
</style>

<script>
import Card from "./components/Card.vue"
import Header from "./components/Header.vue"

export default ({
  components: { Card, Header },
  setup() {
    components: { Card, Header }
  },
})
</script>





