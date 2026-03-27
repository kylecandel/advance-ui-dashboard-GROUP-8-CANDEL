<template>
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
</template>

<style scoped>
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
</style>