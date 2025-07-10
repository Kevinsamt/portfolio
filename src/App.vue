<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header class="main-header">
    <img src="/vite.svg" class="logo" alt="Vite logo" />
    <h1 class="brand-title">Kevin Samuel T</h1>
    <nav>
      <a href="#" class="nav-link">Home</a>
      <a href="#" class="nav-link">About</a>
      <a href="#" class="nav-link">Contact</a>
    </nav>
  </header>
  <main class="main-content">
    <HelloWorld msg="Selamat Datang di Portfolio Kevin Samuel T" />
  </main>
  <footer class="main-footer">
    <span>© 2024 Kevin Samuel T. All rights reserved.</span>
    <span class="footer-links">
      <a href="#">Instagram</a> |
      <a href="#">LinkedIn</a>
    </span>
  </footer>
</template>

<style scoped>
.main-header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  background: linear-gradient(90deg, #646cff 0%, #42b883 100%);
  padding: 1.5rem 2rem;
  box-shadow: 0 2px 12px rgba(0,0,0,0.08);
  border-radius: 0 0 18px 18px;
}
.logo {
  height: 3em;
  margin-right: 1.5em;
}
.brand-title {
  font-size: 2rem;
  color: #fff;
  letter-spacing: 2px;
  font-weight: bold;
  flex: 1;
}
nav {
  display: flex;
  gap: 1.5rem;
}
.nav-link {
  color: #fff;
  font-weight: 500;
  text-decoration: none;
  transition: color 0.2s;
}
.nav-link:hover {
  color: #ffd700;
}
.main-content {
  margin-top: 2.5rem;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.main-footer {
  margin-top: 3rem;
  padding: 1.2rem 2rem;
  background: linear-gradient(90deg, #42b883 0%, #646cff 100%);
  color: #fff;
  text-align: center;
  border-radius: 18px 18px 0 0;
  font-size: 1.05rem;
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
  box-shadow: 0 -2px 12px rgba(0,0,0,0.06);
}
.footer-links a {
  color: #ffd700;
  text-decoration: none;
  margin: 0 0.3rem;
  font-weight: 500;
  transition: color 0.2s;
}
.footer-links a:hover {
  color: #fff;
  text-decoration: underline;
}
</style>
