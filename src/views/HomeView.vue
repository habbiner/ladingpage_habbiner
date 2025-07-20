<script setup>
import { useRouter } from 'vue-router';

const router = useRouter();

function handleContactClick() {
  alert('Ta clicando, só falta fazer a outra tela.');
}
</script>

<template>
  <div>
    <main>
      <img src="/src/assets/logo-bg.png" alt="Logo HA Solutions" />
      <nav>
        <span>QUEM SOMOS</span>
        <span>SERVIÇOS</span>
        <span>PROJETOS</span>
        <span>ORÇAMENTO</span>
        <button @click="handleContactClick">CONTATE-NOS</button>
      </nav>
    </main>

    <header>
      <video src="/src/assets/vd01.mp4" autoplay muted loop playsinline></video>
      <div class="header-content">
        <h1>Conectando ideias à tecnologia</h1>
        <h3>Transformando sua visão em realidade com projetos personalizados</h3>
      </div>
    </header>

    <section class="content">
      <h2>HA Solutions - Soluções em tecnologia</h2>
      <p>Com mais de 5 anos de experiência em desenvolvimento de sistemas, infraestrutura e projetos personalizados.</p>
    </section>
  </div>
</template>

<style scoped>
main {
  position: fixed;
  top: 0;
  width: 100%;
  height: 10vh;
  background-color: #0D1B2A;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 2rem;
  z-index: 10;
}

main img {
  width: 8%;
  max-width: 80px;
}

nav {
  display: flex;
  align-items: center;
  gap: 1.5rem;
}

span,
button {
  font-family: Poppins, Montserrat, Roboto, sans-serif;
  color: white;
  font-size: 1em;
  cursor: pointer;
}

button {
  background-color: #3F72AF;
  border: none;
  padding: 0.5rem 1rem;
  border-radius: 5px;
  transition: 0.3s;
}

button:hover {
  background-color: #518fd6;
}

header {
  position: relative;
  height: 100vh;
  margin-top: 10vh;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
}

header video {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  z-index: -1;
}

.header-content {
  color: white;
  text-align: center;
  padding: 0 2rem;
}

.header-content h1 {
  font-size: 3rem;
  font-family: Montserrat, sans-serif;
}

.header-content h3 {
  font-size: 1.5rem;
  font-family: Poppins, sans-serif;
  margin-top: 1rem;
}

.content {
  padding: 4rem 2rem;
  background-color: #f4f4f4;
  text-align: center;
  font-family: Roboto, sans-serif;
}

.content h2 {
  color: #0D1B2A;
  font-size: 2rem;
  margin-bottom: 1rem;
}

.content p {
  color: #333;
  font-size: 1.2rem;
}
</style>
