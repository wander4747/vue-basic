<template>
    <div>
        <p v-if="isWorking">Está trabalhando</p>
        <p v-else>Não está trabalhando</p>
        <p>Tecnologias</p>
        <ul>
            <li>PHP</li>
            <li>GO</li>
        </ul>
        <p v-show="showEmail">Email é: teste@test.com</p>
    </div>
    
</template>

<script>
export default {
    name: 'Info',
    data() {
        return {
            isWorking: true,
            showEmail: true
        }
    }
}
</script>