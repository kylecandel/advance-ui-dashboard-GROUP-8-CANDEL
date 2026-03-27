<script setup>
</script>

<template>

  <div class="dashboard">
    <header class="header">Header</header>

    <aside class="sidebar">
  <nav aria-label="Main Navigation">
    <ul>
      <li><button aria-label="Go to Dashboard">Dashboard</button></li>
      <li><button aria-label="View Users">Users</button></li>
      <li><button aria-label="View Reports">Reports</button></li>
      <li><button aria-label="Open Settings">Settings</button></li>
    </ul>
  </nav>
</aside>

<main class="main" role="main">
  <div class="cards">

    <div class="card">
      <button aria-label="View Users Statistics">Users</button>
    </div>

    <div class="card">
      <button aria-label="View Sales Data">Sales</button>
    </div>

    <div class="card">
      <button aria-label="View Revenue Data">Revenue</button>
    </div>

    <div class="card">
      <button aria-label="View Performance Metrics">Performance</button>
    </div>

  </div>
</main>
    <footer class="footer">Footer</footer>
  </div>
</template>









<style>
.dashboard {
  display: grid;
  grid-template-columns: 1fr;
  grid-template-areas:
    "header"
    "sidebar"
    "main"
    "footer";
  gap: 10px;
  padding: 10px;
}

.header {
  grid-area: header;
  background: #1e293b;
  color: white;
  padding: 20px;
}

.sidebar {
  grid-area: sidebar;
  background: #334155;
  color: white;
  padding: 20px;
}

.main {
  grid-area: main;
  background: #475569;
  color: white;
  padding: 20px;
}

.footer {
  grid-area: footer;
  background: #0f172a;
  color: white;
  padding: 20px;
}

.cards {
  display: grid;
  grid-template-columns: 1fr;
  gap: 10px;
}

.card {
  background: #1e293b;
  padding: 20px;
  border-radius: 8px;
  color: white;
  text-align: center;
  font-weight: bold;
}

.sidebar ul {
  list-style: none;
  padding: 0;
}

.sidebar li {
  margin-bottom: 10px;
}

.sidebar button {
  width: 100%;
  padding: 10px;
  border: none;
  background: #1e293b;
  color: white;
  border-radius: 6px;
  cursor: pointer;
}

.sidebar button:hover {
  background: #0f172a;
}

.card button {
  width: 100%;
  padding: 15px;
  border: none;
  background: transparent;
  color: white;
  font-size: 16px;
  cursor: pointer;
}

button:focus {
  outline: 3px solid #38bdf8;
}

@media (min-width: 768px) {
  .dashboard {
    grid-template-columns: 200px 1fr;
    grid-template-areas:
      "header header"
      "sidebar main"
      "footer footer";
  }

  @media (min-width: 768px) {
  .cards {
    grid-template-columns: repeat(2, 1fr);
  }
}


}
</style>