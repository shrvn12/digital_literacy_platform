<template>
  <section>
    <h1 class="page-title">📚 Curriculum</h1>
    <p class="subtitle">6 Units · 42 Lessons · Grades 3–8 · Learn coding step by step!</p>
    <div class="panel">
      <h2 style="font-size:22px;margin-top:0">🌱 Unit 1: Introduction to Computers <span class="pill">BEGINNER</span></h2>
      <ol style="font-size:22px;line-height:1.6;margin:0;padding-left:30px">
        <li v-for="l in lessons" :key="l">{{ l }}</li>
      </ol>
    </div>
  </section>
</template>

<script setup>
const lessons = [
  'What is a Computer?',
  'Input & Output Devices',
  'The Internet — What is it?',
  'Files & Folders',
  'Typing & Keyboard Skills',
  'Digital Safety & Privacy',
  'Unit 1 Quiz & Badge'
]
</script>
