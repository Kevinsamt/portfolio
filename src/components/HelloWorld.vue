<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
  <div class="hello-card">
    <h1 class="hello-title">{{ msg }}</h1>
    <div class="card-content">
      <button type="button" class="modern-btn" @click="count++">Klik Saya ({{ count }})</button>
      <p class="desc">
        Ini adalah contoh komponen Vue. Edit <code>components/HelloWorld.vue</code> untuk mulai bereksperimen!
      </p>
    </div>
    <div class="links">
      <a href="https://vuejs.org/guide/quick-start.html#local" target="_blank">Panduan Vue</a>
      <a href="https://vitejs.dev/guide/" target="_blank">Panduan Vite</a>
    </div>
  </div>
</template>

<style scoped>
.hello-card {
  background: #fff;
  border-radius: 18px;
  box-shadow: 0 4px 24px rgba(100, 108, 255, 0.10), 0 1.5px 6px rgba(66, 184, 131, 0.08);
  padding: 2.5rem 2rem 2rem 2rem;
  max-width: 420px;
  margin: 0 auto;
  text-align: center;
  transition: box-shadow 0.3s;
}
.hello-card:hover {
  box-shadow: 0 8px 32px rgba(100, 108, 255, 0.18), 0 3px 12px rgba(66, 184, 131, 0.12);
}
.hello-title {
  font-size: 2.2rem;
  color: #646cff;
  margin-bottom: 1.2rem;
  font-weight: bold;
}
.card-content {
  margin-bottom: 1.5rem;
}
.modern-btn {
  background: linear-gradient(90deg, #646cff 0%, #42b883 100%);
  color: #fff;
  border: none;
  border-radius: 8px;
  padding: 0.7em 1.5em;
  font-size: 1.1em;
  font-weight: 600;
  cursor: pointer;
  box-shadow: 0 2px 8px rgba(100, 108, 255, 0.10);
  transition: background 0.2s, transform 0.2s;
}
.modern-btn:hover {
  background: linear-gradient(90deg, #42b883 0%, #646cff 100%);
  transform: translateY(-2px) scale(1.04);
}
.desc {
  color: #555;
  margin-top: 1.2rem;
  font-size: 1.05rem;
}
.links {
  display: flex;
  justify-content: center;
  gap: 1.5rem;
  margin-top: 1.5rem;
}
.links a {
  color: #646cff;
  font-weight: 500;
  text-decoration: none;
  transition: color 0.2s;
}
.links a:hover {
  color: #42b883;
}
</style>
