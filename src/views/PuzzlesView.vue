<template>
  <section>
    <h1 class="page-title">🧩 Puzzles</h1>
    <p class="subtitle">Logic puzzles, drag-and-drop challenges, and code jumbles!</p>
    <div class="cards-3">
      <article class="card" v-for="p in puzzles" :key="p.title">
        <div class="card-cover">{{ p.icon }}</div>
        <div class="card-body">
          <h3>{{ p.title }}</h3>
          <p>{{ p.desc }}</p>
          <button class="btn primary" style="width:100%">{{ p.cta }}</button>
        </div>
      </article>
    </div>
  </section>
</template>

<script setup>
const puzzles = [
  { icon: '🔀', title: 'Code Unjumbler', desc: 'Rearrange lines into a working program!', cta: '🧩 Solve It!' },
  { icon: '🐛', title: 'Bug Hunt', desc: 'Spot bugs in broken snippets.', cta: '🐍 Find Bugs!' },
  { icon: '🔗', title: 'Match the Blocks', desc: 'Match Scratch blocks to Python code.', cta: '🔗 Match Now!' }
]
</script>
