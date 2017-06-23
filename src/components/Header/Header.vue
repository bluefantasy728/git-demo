<template>
  <div>
    <h3>{{seller.name}}</h3>
    <img :src="seller.avatar" width="64" height="64"/>
    <ul v-if="seller.supports">
      <li>{{seller.supports[0].description}}</li>
    </ul>
  </div>
</template>

<script>
export default {
  props: {
    seller: {
      type: Object
    }
  }
}
</script>

<style lang="scss">

</style>
