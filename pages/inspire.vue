<template>
  <div>
    <h1>Hell, nuxt</h1>
    <form @submit.prevent="route()">
      <input v-model="q" type="text" />
      <button>검색 페이지로</button>
    </form>
  </div>
</template>

<script>
export default {
  data: () => ({
    q: '',
  }),
  methods: {
    route() {
      this.$router.push('/search')
    },
  },
}
</script>
