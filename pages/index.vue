<template>
  <section class="container">
    <div>
      <h1 class="title">
        Home
      </h1>
      <h2 class="subtitle">
        Nuxt.js home page
      </h2>
      <div class="links">
        <nuxt-link to="/about" class="button--green">About</nuxt-link>
      </div>
      <div class="links">
        <nuxt-link to="/api" class="button--green">API</nuxt-link>
      </div>
    </div>
  </section>
</template>

<script>
export default {
}
</script>

<style scoped>
.container {
  display: flex;
  justify-content: center;
  text-align: center;
}

.title {
  font-family: -apple-system, "Helvetica Neue", sans-serif;
  display: block;
  font-weight: 300;
  font-size: 70px;
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

