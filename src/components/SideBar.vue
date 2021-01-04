<template>
  <nav class="sidebar" :class="open ? 'open' : 'closed'">
    <ul class="sidebar-list">
      <li class="sidebar-list__item logo">
        <a href="javascript:void(0)" class="sidebar-list__link">
          <img src="../assets/images/logo.svg" alt="" width="20">
          stocklabs
        </a>
      </li>
      <li class="sidebar-list__item search">
        <div class="expand-icon icon-arrow-right-c" @click="open = true">
        </div>
        <a href="javascript:void(0)" class="sidebar-list__link">Search</a>
      </li>
      <li class="sidebar-list__item">
        <a href="javascript:void(0)" class="sidebar-list__link">Home</a>
      </li>
      <li class="sidebar-list__item">
        <a href="javascript:void(0)" class="sidebar-list__link">Market View</a>
      </li>
      <li class="sidebar-list__item">
        <a href="javascript:void(0)" class="sidebar-list__link">News</a>
      </li>
      <li class="sidebar-list__item">
        <a href="javascript:void(0)" class="sidebar-list__link">Industries</a>
      </li>
      <li class="sidebar-list__item">
        <a href="javascript:void(0)" class="sidebar-list__link">Screencer</a>
      </li>
      <li class="sidebar-list__item">
        <a href="javascript:void(0)" class="sidebar-list__link">Watch list</a>
      </li>
      <li class="sidebar-list__item">
        <a href="javascript:void(0)" class="sidebar-list__link">Chat</a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'SideBar',
  data () {
    return {
      open: false
    }
  }
}
</script>
