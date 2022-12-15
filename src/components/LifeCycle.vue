<template>
    <h2>Meu nome é: {{ name }}</h2>
</template>

<script>
export default {
    name: "Lifecycle",
    data() {
        return {
            name: "Lifecycle",
        }
    },
    created() {
        setTimeout(() => {
            this.name = "Lifecycle created"
        }, 1000);
    },
    mounted() {
        setTimeout(() => {
            this.name = "Lifecycle mounted"
        }, 2000);
    }
}
</script>
