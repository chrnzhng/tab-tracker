<template>
  <div>
    <h1>Register</h1>

    <input 
    type="email" 
    name="email" 
    v-model ="email"
    placeholder="email" />
    <br>
    <input 
    type="password" 
    name="password" 
    v-model="password"
    placeholder="password" />
    <br>
    <button>Register</button>
  </div>
</template>

<script>
export default {
  data () {
    return {
      email: 'abc',
      password: '123'
    }
  },
  watch: {
    email (value) {
      console.log('email has changed', value)
    }
  },
  mounted () {
    setTimeout(() => {
      this.email = 'hello world'
    }, 2000)
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
