<template>
  <h1>The sidebar is {{ collapsed ? 'closed' : 'open' }}</h1>
  <button @click="toggleSidebar">Toggle Sidebar</button>
</template>

<script>
import { collapsed, toggleSidebar } from '@/components/state'

export default {
  name: "DashboardView",
  setup() {
    return { collapsed, toggleSidebar }
  }
}
</script>