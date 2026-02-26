<template>
  <section>
    <div class="hero">
      <div>
        <h2>Welcome back, Shravan! 👋</h2>
        <p>You're on a 🔥 5-day streak! Continue where you left off — you're 65% through <strong style="color:#ffb41f">Unit 3: Loops & Logic</strong></p>
        <div class="btn-row">
          <button class="btn primary">▶ Continue Learning</button>
          <button class="btn ghost">🧠 Quick Quiz</button>
        </div>
      </div>
      <div style="font-size:100px">🌱</div>
    </div>

    <div class="grid-4">
      <article class="stat" v-for="item in stats" :key="item.label" :style="{borderBottomColor:item.color}">
        <h3>{{ item.icon }}</h3>
        <div class="num">{{ item.value }}</div>
        <p class="subtitle" style="margin:0;font-size:20px">{{ item.label }}</p>
      </article>
    </div>
  </section>
</template>

<script setup>
const stats = [
  { icon: '⭐', value: '1,240', label: 'Total XP Earned', color: '#16a9f5' },
  { icon: '📖', value: '18', label: 'Lessons Done', color: '#30c05f' },
  { icon: '🏅', value: '7', label: 'Badges Earned', color: '#e760b2' },
  { icon: '🔥', value: '5', label: 'Day Streak', color: '#fb9a11' }
]
</script>
