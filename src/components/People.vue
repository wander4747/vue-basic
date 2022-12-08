<template>
    <div>
        <h2>Descrição do {{ name }}</h2>
        <Info />
    </div>
    
</template>

<script>
import Info from "./Info";

export default {
    name: 'People',
    components: {
        Info
    },
    data() {
        return {
            name: 'Wander'
        }
    }
}
</script>