<template>
    <div>
        <p v-if="isWorking">Está trabalhando</p>
        <p v-else>Não está trabalhando</p>
        <p>Tecnologias</p>
        <ul>
            <li v-for="(language, index) in languages" :key="index">{{ language }}</li>
        </ul>
        <p>Tecnologias objeto</p>
        <ul>
          <li v-for="language in languagesObject" :key="language.id">{{ language.name }}</li>
        </ul>
        <div>
          <button @click="showEmail()">Mostrar email</button>
        </div>
        <p v-show="showEmailParagraph">Email é: {{ email }}</p>
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
    props: {
      email: String
    },
    data() {
        return {
            isWorking: true,
            showEmailParagraph: true,
            site: "https://www.google.com",
            languages:['PHP', 'GO', 'Node'],
            languagesObject: [
              { id: 1, name : 'PHP'},
              { id: 2, name : 'GO'},
              { id: 3, name : 'Node'},
            ]
        }
    },
    methods: {
      showEmail() {
        this.showEmailParagraph = !this.showEmailParagraph
      }
  }
}
</script>
