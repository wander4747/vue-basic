<template>
    <div>
        <h2>Descrição do {{ name }}</h2>
        <Info :email="email"/>
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
            name: 'Wander',
            email: 'test@test.com'
        }
    }
}
</script>
