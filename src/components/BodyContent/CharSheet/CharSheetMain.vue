<template>
  <div class="char-sheet">
    <Card
      :currentComponent="'Header'"
      :XStart="1"
      :XEnd="10"/>
    <Card
      :currentComponent="'Abilities'"
      :YStart="2"
      :YEnd="5"/>
    <Card
      :currentComponent="'SavingThrows'"
      :XStart="2"
      :XEnd="4"/>
    <Card
      :currentComponent="'ArmorClass'"
      :XStart="4"
      :XEnd="7"
      :YStart="2"
      :YEnd="4"/>
    <Card
      :currentComponent="'HitPoints'"
      :XStart="7"
      :XEnd="10"
      :YStart="2"/>
    <Card
      :currentComponent="'Skills'"
      :XStart="2"
      :XEnd="4"
      :YStart="3"
      :YEnd="5"/>
    <Card
      :currentComponent="'Proficiencies'"
      :XStart="7"
      :XEnd="10"/>
    <Card
      :currentComponent="'Actions'"
      :XStart="4"
      :XEnd="10"/>
    <Card
      :currentComponent="'Senses'"
      :XStart="1"
      :XEnd="4"/>
    <Card
      :currentComponent="'Attacks'"
      :XStart="4"
      :XEnd="10"/>
  </div>
</template>

<script>

import Card from './Card.vue'
export default {
  name: 'CharSheetMain',
  components: {
    Card
  },
  data () {
    return {
    }
  },
  methods: {
  }
}
</script>

<style scoped lang="scss">
.char-sheet {
  min-height: 88.571429em;
  max-height: 88.571429em;
  min-width: 62.428571em;
  max-width: 62.428571em;
  border: 2px solid black;
  margin: 0 auto;
  padding: 1em 3em 3em;
  display: grid;
  grid-template-columns: repeat(9, 1fr);
  grid-template-rows: .5fr repeat(4, 1fr);
}
</style>
