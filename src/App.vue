<template>
  
  <div>
    <h3>Matriz original:</h3>
    <table>
      <tr v-for="(linha, indexLinha) in matriz" :key="indexLinha">
        <td v-for="(valor, indexColuna) in linha" :key="indexColuna">
          {{ valor }},
        </td>
      </tr>
    </table>

    <h3>Matriz resultante:</h3>
    <table>
      <tr v-for="(linha, indexLinha) in matrizResultante" :key="indexLinha">
        <td v-for="(valor, indexColuna) in linha" :key="indexColuna">
          {{ valor }},
        </td>
      </tr>
    </table>
  </div>
</template>

<script>

let numero1 = Number(prompt("informe um numero"))
let numero2 = Number(prompt("informe um numero"))
let numero3 = Number(prompt("informe um numero"))
let numero4 = Number(prompt("informe um numero"))
let numero5 = Number(prompt("informe um numero"))
let numero6 = Number(prompt("informe um numero"))
let numero7 = Number(prompt("informe um numero"))
let numero8 = Number(prompt("informe um numero"))
let numero9 = Number(prompt("informe um numero"))

let numeromult = Number(prompt("informe o numero de vai multiplicar as matrizes"))

export default {
  data() {
    return {
      matriz: [[numero1, numero2, numero3], [numero4, numero5, numero6], [numero7, numero8, numero9]],
      numero: numeromult,
      matrizResultante: [],
    };
  },
  mounted() {
    this.multiplicarMatrizPorNumero();
  },
  methods: {
    multiplicarMatrizPorNumero() {
      this.matrizResultante = this.matriz.map((linha) =>
        linha.map((valor) => valor * this.numero)
      );
    },
  },
};
</script>
<style>
table {
  padding: 10%;
  background-color: aliceblue;
  font-size: xx-large;
  border-radius: 5%;
  border: 1.5px solid black;
}

h3 {
  color: aliceblue;
}
</style>