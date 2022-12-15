<template>
    <button @click="$emit('eventChangeImage')">Mudar imagem</button>
</template>

<script>
export default {
  name: 'ButtonImage',
  emits: ['eventChangeImage'],
}
</script>
