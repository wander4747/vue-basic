<template>
    <div>
        <h1>Hello Vue</h1>
        <p>Meu nome é {{ name }} e trabalho como {{ job }}</p>
    </div>
</template>

<script>
export default {
    name: 'FirstComponent',
    data() {
        return {
            name: "Wander",
            job: "Developer"
        }
    }
}
</script>
