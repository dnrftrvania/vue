<template>
  <div id="app">
  <div id="main-wrapper" data-navbarbg="skin6" data-theme="light" data-layout="vertical" data-sidebartype="full" data-boxed-layout="full">
    <div class="topbar" data-navbarbg="skin6">
      <router-view name="navbar" />
    </div>
    <div class="left-sidebar" data-sidebarbg="skin5">
      <router-view name="sidebar" />
    </div>
  </div>
      <div class="page-wrapper">
        <router-view />
      </div>
    <router-view name="footer" />
  </div>
</template>

<script>
import Navbar from './views/layouts/Navbar'
import Sidebar from './views/layouts/Sidebar'
export default {
  name: 'App',
  components: {
    Navbar
  }
}
</script>
