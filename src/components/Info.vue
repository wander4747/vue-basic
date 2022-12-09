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
        <p>Para acessar meu portfólio <a v-bind:href="site" target="_blank">clique aqui</a></p>
        <Picture />
    </div>
    
</template>

<script>
import Picture from "./Picture";

export default {
    name: 'Info',
    components: {
        Picture
    },
    data() {
        return {
            isWorking: true,
            showEmail: true,
            site: "https://www.google.com"
        }
    }
}
</script>