<template>
    <img :src="avatar" />
</template>

<script>
import Info from "./Info";

export default {
    name: 'Picture',
    data() {
        return {
            avatar: '/img/logo.png'
        }
    }
}
</script>
