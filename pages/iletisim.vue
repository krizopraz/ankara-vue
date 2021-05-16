<template>
  <div>
    <form prevent action="">
      <input v-model.lazy="name" type="text">
      <input v-model.lazy="surname" type="text">
      <input v-model.lazy="email" type="email">
      <input type="button" value="Katıl!" @click="joinnow">
    </form>
  </div>
</template>

<script>
export default {
  data () {
    return {
      name: '',
      surname: '',
      email: ''
    }
  },
  methods: {
    joinnow () {
      this.name = null
      this.surname = null
      this.email = null
      return true
    }
  }
}
</script>

<style lang="scss" scoped>
div{
  padding-top: 30vh;
}
</style>
