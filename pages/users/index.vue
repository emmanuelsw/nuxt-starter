<template>
  <section class="container">
    <div>
      <h1 class="title">
        Users
      </h1>
      <p>{{ip}}</p>
      <nuxt-link to="/" class="button--green">Home</nuxt-link>
    </div>

  </section>
</template>

<script>
export default {
  data() {
    return {
      message: ''
    }
  },
  async asyncData({ app }) {
    const ip = await app.$axios.$get('http://icanhazip.com')
    return { ip: ip, message: ip }
  }
}
</script>

<style scoped>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  padding-top: 20px;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 40px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>

