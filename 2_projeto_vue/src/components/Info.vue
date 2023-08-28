<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Estou em busca de novas oportunidades!</p>
        <p>Utilizo as seguintes tecnologias:</p>
    <ul>
    <li>Javascript</li>
    <li>PHP</li>
    <li>Python</li>
   </ul>
  <p>Mande uma mensagem para: {{ email }}</p>
</div>
</template>

<script lang="js">
export default {
    name: 'Info',
    data() {
        return {
            esta_trabalhando: false,
            mostrar_email: true
        }
    }
}
</script>