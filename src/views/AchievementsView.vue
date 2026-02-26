<template>
  <section>
    <h1 class="page-title">🏆 Achievements</h1>
    <p class="subtitle">Earn badges by completing lessons, quizzes, and challenges!</p>
    <div class="panel">
      <h2 style="font-size:50px;margin-top:0">🌟 Badges Earned (7 / 18)</h2>
      <div class="cards-3" style="grid-template-columns:repeat(4,1fr)">
        <div class="panel" v-for="b in badges" :key="b" style="text-align:center;padding:14px">
          <div style="font-size:72px">{{ b.icon }}</div>
          <strong style="font-size:28px">{{ b.name }}</strong>
        </div>
      </div>
      <h2 style="font-size:46px">📈 XP Milestones</h2>
      <p style="font-size:34px;margin:0 0 12px">Level 3 – Code Explorer <span style="float:right">1,240 / 1,500 XP</span></p>
      <div class="progress"><span style="width:82%" /></div>
    </div>
  </section>
</template>

<script setup>
const badges = [
  { icon: '🌱', name: 'First Login!' },
  { icon: '💻', name: 'Digital Explorer' },
  { icon: '🤖', name: 'Algorithm Ace' },
  { icon: '🔥', name: '5-Day Streak' }
]
</script>
