<template>
  <nav class="sidebar" :class="open ? 'open' : 'closed'">
    <ul class="sidebar-list">
      <li class="sidebar-list__item logo">
        <a href="javascript:void(0)" class="sidebar-list__link">
          <img src="../assets/images/logo.svg" alt="" width="20">
          <transition name="fade-in">
            <span v-if="open" class="ml-2 logo-name">stocklabs</span>
          </transition>
        </a>
      </li>
      <li class="sidebar-list__item">
        <div class="expand-icon icon-arrow-right" @click="open = ! open" :class="open && 'open'">
        </div>
        <a href="javascript:void(0)" class="sidebar-list__link">
          <span class="icon-search"></span>
          <transition name="fade-in">
            <span v-if="open" class="ml-2">Search</span>
          </transition>
        </a>
      </li>
      <li class="sidebar-list__item">
        <a href="javascript:void(0)" class="sidebar-list__link">
          <span class="icon-home"></span>
          <transition name="fade-in">
            <span v-if="open" class="ml-2">Home</span>
          </transition>
        </a>
      </li>
      <li class="sidebar-list__item">
        <a href="javascript:void(0)" class="sidebar-list__link">
          <span class="icon-bar-chart"></span>
          <transition name="fade-in">
            <span v-if="open" class="ml-2">Market View</span>
          </transition>
        </a>
      </li>
      <li class="sidebar-list__item">
        <a href="javascript:void(0)" class="sidebar-list__link">
          <span class="icon-bell-on"></span>
          <transition name="fade-in">
            <span v-if="open" class="ml-2">News</span>
          </transition>
        </a>
      </li>
      <li class="sidebar-list__item">
        <a href="javascript:void(0)" class="sidebar-list__link">
          <span class="icon-calendar"></span>
          <transition name="fade-in">
            <span v-if="open" class="ml-2">Industries</span>
          </transition>
        </a>
      </li>
      <li class="sidebar-list__item">
        <a href="javascript:void(0)" class="sidebar-list__link">
          <span class="icon-cast"></span>
          <transition name="fade-in">
            <span v-if="open" class="ml-2">Screencer</span>
          </transition>
        </a>
      </li>
      <li class="sidebar-list__item">
        <a href="javascript:void(0)" class="sidebar-list__link">
          <span class="icon-compass"></span>
          <transition name="fade-in">
            <span v-if="open" class="ml-2">Watch list</span>
          </transition>
        </a>
      </li>
      <li class="sidebar-list__item">
        <a href="javascript:void(0)" class="sidebar-list__link">
          <span class="icon-folder"></span>
          <transition name="fade-in">
            <span v-if="open" class="ml-2">Chat</span>
          </transition>
        </a>
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
