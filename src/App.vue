<template>
  <div class="app-shell">
    <aside class="sidebar">
      <div class="brand">
        <h1>Code<span>Kids</span> 🚀</h1>
        <p>Digital Literacy Platform</p>
      </div>

      <div class="nav-group">
        <small>LEARN</small>
        <RouterLink to="/" class="nav-item">🏠 Home</RouterLink>
        <RouterLink to="/curriculum" class="nav-item">📚 Curriculum</RouterLink>
        <RouterLink to="/lessons" class="nav-item">💡 Lessons</RouterLink>
        <RouterLink to="/playground" class="nav-item">🎮 Playground</RouterLink>
      </div>

      <div class="nav-group">
        <small>PLAY</small>
        <RouterLink to="/games" class="nav-item">🕹️ Games</RouterLink>
        <RouterLink to="/quizzes" class="nav-item">🧠 Quizzes</RouterLink>
        <RouterLink to="/puzzles" class="nav-item">🧩 Puzzles</RouterLink>
      </div>

      <div class="nav-group">
        <small>PROGRESS</small>
        <RouterLink to="/achievements" class="nav-item">🏆 Achievements</RouterLink>
      </div>
    </aside>

    <main class="content">
      <RouterView />
    </main>
  </div>
</template>
