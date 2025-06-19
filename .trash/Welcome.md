
```vue

<script setup lang="ts">
const title = 'Edgar Allan Poe'
const description =
  'Edgar Allan Poe foi um escritor, poeta, editor e crítico literário norte-americano, considerado um dos mestres do conto de terror e do mistério. Nascido em 19 de janeiro de 1809, em Boston, Massachusetts, Poe é amplamente reconhecido por suas contribuições à literatura gótica e por ser um precursor do gênero policial. Suas obras mais conhecidas incluem "O Corvo", "O Gato Preto" e "O Coração Delator". Poe faleceu em 7 de outubro de 1849, em circunstâncias misteriosas, deixando um legado duradouro na literatura mundial.'
const telefone = '920 551 268'
const fullname = 'Michifus'
const imageUrl = 'https://cataas.com/cat'
</script>

<template>
  <div class="app-container">
    <header class="header-container">
      <h1 class="title">{{ title }}</h1>
    </header>
    <p class="description">
      {{ description }}
    </p>
    <div class="container">
      <div class="card">
        <div class="bloque-1">
          <div class="data-nombre">
            <div><strong>Nombre:</strong></div>
            <div class="const-fn">{{ fullname }}</div>
          </div>
          <div class="data-number">
            <div><strong>Telefono:</strong></div>
            <div class="const-tf">{{ telefone }}</div>
          </div>
        </div>
        <div class="bloque-2"></div>
      </div>
    </div>
  </div>
</template>
<style scoped>
.card {
  display: flex;
  gap: 2px;
  width: 600px;
  height: 350px;
  border-radius: 50px;
  background-color: rgb(235, 187, 235);
  border: 4px solid rgb(181, 0, 181);
  box-shadow: 0 5px  10px rgba(182, 124, 178, 0.679);
}
.bloque-1,
.bloque-2 {
  padding: 1rem;
}
.bloque-1 {
  flex: 1;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.bloque-2 {
  flex: 1.5;
  display: flex;
  align-items: center;
  justify-content: center;
  background-image: url('https://cataas.com/cat');
  background-size: cover;
  background-position: center;
  border-radius: 10%;
  border: 3px solid rgb(181, 0, 181);
}
strong {
  font-size: 22px;
  color: rgb(179, 14, 179);
}
.const-fn,
.const-tf {
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.2rem;
  border-radius: 40px;
  border: 3px dashed rgb(181, 0, 181);
  background-color: rgb(245, 213, 241);
  font-size: 18px;
}

.data-nombre,
.data-number {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

* {
  /* border: 1px solid gray; */
  padding: 5px;
  margin: 5px;
}

.title {
  font-size: 2.5rem;
  text-align: center;
}
.description {
  font-size: 1rem;
  text-align: center;
}
.header-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 1rem;
  width: 100%;
}
.app-container {
  width: 100%;
  display: flex;
  flex-direction: column;
}
</style>

```