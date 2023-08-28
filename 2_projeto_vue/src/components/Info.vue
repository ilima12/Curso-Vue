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
  <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
  <p>Para acessar meu portfólio basta clicar aqui <a v-bind:href="meu_link" target="_blank">basta clicar aqui</a></p>
</div>
</template>

<script lang="js">
export default {
    name: 'Info',
    data() {
        return {
            esta_trabalhando: false,
            mostrar_email: true,
            email: 'italo@gmail.com',
            meu_link: 'https://google.com'
        }
    }
}
</script>