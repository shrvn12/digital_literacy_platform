<template>
  <section>
    <h1 class="page-title">🕹️ Games</h1>
    <p class="subtitle">Learn programming concepts through fun games!</p>
    <div class="cards-3">
      <article class="card" v-for="g in games" :key="g.title">
        <div class="card-cover" :style="{background:g.color}">{{ g.icon }}</div>
        <div class="card-body">
          <h3>{{ g.title }}</h3>
          <p>{{ g.desc }}</p>
          <button class="btn primary" style="width:100%">▶ Play Now</button>
        </div>
      </article>
    </div>
  </section>
</template>

<script setup>
const games = [
  { icon: '🐢', title: 'Turtle Maze Runner', desc: 'Guide a turtle through a maze with sequences!', color: '#272a73' },
  { icon: '🥭', title: 'Catch the Mango!', desc: 'Use loops to catch falling mangoes.', color: '#18763a' },
  { icon: '🤖', title: 'Robot Factory', desc: 'Program robots with if-else conditions.', color: '#9e330f' }
]
</script>
