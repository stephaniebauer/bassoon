<template>
  <div class="riddleBackground">
    <div class="houseContainer" @click="openHouseRiddle">
      <img src="https://toppng.com/uploads/preview/transparent-background-house-11549431583jinu4eokqc.png" alt="" class="house">
    </div>
    <div class="finishLineContainer" @click="openFinishLineRiddle">
      <img src="../assets/finish.png" alt="" class="finishLine">
    </div>
  </div>
</template>

<script>
export default {
  name: 'riddleView',
  methods: {
    openHouseRiddle () {
      alert('¡Hola!')
    },
    openFinishLineRiddle () {
      alert('¡Adios!')
    }
  }
}
</script>

<style lang="sass">
  img
    width: 128px
    aspect-ratio: 1 / 1
    cursor: pointer

  .riddleBackground
    position: relative
    width: auto
    height: 100vh
    background-size: cover
    background-image: url(../assets/landscape.jpg)

  .house
    position: absolute
    bottom: 5vh
    left: 15vw

  .finishLine
    position: absolute
    bottom: 25vh
    right: 10vw
</style>
