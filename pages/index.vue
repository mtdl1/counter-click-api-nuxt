<script setup>
const handleClick = async () => {
  const res = await fetch('/api/count', {
    method: 'POST',
    body: JSON.stringify({}),
  })
  const data = await res.json()
  console.log(data)
}
</script>

<template>
  <button @click="handleClick">Click me</button>
</template>