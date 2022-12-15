<template>
    <img :src="avatar" @eventChangeImage="changeImage()"/>
    <ButtonImage @event-change-image="changeImage"/>
</template>

<script>

import ButtonImage from "./ButtonImage";

export default {
    name: 'Picture',
    components: {
        ButtonImage
    },
    emits: ['eventChangeImage'],
    data() {
        return {
            avatar: '/img/logo.png'
        }
    },
    methods: {
      changeImage() {
        this.avatar = '/img/avatar.png'
      }
    }
}
</script>
