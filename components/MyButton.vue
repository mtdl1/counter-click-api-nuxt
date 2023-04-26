<template>
  <button class="btn btn-primary" @click="handleClick">clique aqui</button>
</template>

<script>
export default {
  name: 'MyButton',
  data() {
    return {
      cliques: 0
    }
  },
  // methods: {
  //   async handleClick() {
  //     this.cliques++
  //     await fetch('/api/whatsapp-clicks', {
  //       method: 'POST',
  //       headers: {
  //         'Content-Type': 'application/json'
  //       },
  //       body: JSON.stringify({
  //         clicks: this.cliques
  //       })
  //     })
  //   }
  // }
}
</script>