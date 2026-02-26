<template>
  <section>
    <h1 class="page-title">💡 Lessons</h1>
    <p class="subtitle">Pick a lesson and start learning at your pace!</p>
    <div class="cards-3">
      <article class="card" v-for="l in cards" :key="l.title">
        <div class="card-cover" :style="{background:l.color}">{{ l.icon }}</div>
        <div class="card-body">
          <span class="pill">{{ l.unit }}</span>
          <h3>{{ l.title }}</h3>
          <p>⏱ {{ l.time }} · ⭐ {{ l.xp }} XP</p>
          <div class="progress"><span :style="{width:l.progress+'%'}" /></div>
        </div>
      </article>
    </div>
  </section>
</template>

<script setup>
const cards = [
  { icon: '💻', title: 'What is a Computer?', unit: 'UNIT 1', time: '15 min', xp: 50, progress: 100, color: '#b7c3e8' },
  { icon: '🌐', title: 'The Internet – What is it?', unit: 'UNIT 1', time: '20 min', xp: 60, progress: 100, color: '#a7dac2' },
  { icon: '🤖', title: 'What is an Algorithm?', unit: 'UNIT 2', time: '15 min', xp: 60, progress: 95, color: '#e5c7de' }
]
</script>
