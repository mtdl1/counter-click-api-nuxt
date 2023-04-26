<template>
  <div>
    <h1>teste</h1>
    <MyButton />
    <p>{{ clicks }}</p>
  </div>
</template>

<script>
export default {
  name: 'contato',
  data() {
    return {
      clicks: null
    }
  },
  async created() {
    const response = await $fetch('/api/whatsapp-clicks')
    console.log(response)
    this.clicks = response.api
  },
}
</script>