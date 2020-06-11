<template>
  <h1>{{ msg }}</h1>
  <button @click="count++">count is: {{ count }}</button>
  <p>Edit <code>components/HelloWorld.vue</code> to test hot module replacement.</p>

  <div class="container">
    <p>Hello Container, styled with sass</p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      count: 0
    }
  }
}
</script>

<style lang="scss">
  .container {
    width: 80%;
    margin: auto;
    text-align: center;

    p {
      color: blue;
      font-size: 2rem;
      font-weight: 600;
    }
  }
</style>
