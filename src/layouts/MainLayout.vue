<template>
  <div class="app-main-layout">
    <Navbar></Navbar>
    <Sidebar></Sidebar>
    <router-view />
  </div>
</template>

<script>
import Navbar from '@/components/app/Navbar'
import Sidebar from '@/components/app/Sidebar'
export default {
  name: 'main-layout',
  components: {
    Navbar, Sidebar
  }
}
</script>