<template>
    <aside class="sidebar-right">
      <i class="sidebar-right__info">SidebarRight</i>
    </aside>
</template>

<script>
export default {
  name: 'SidebarRight',
  components: {}
}
</script>

<style lang="scss">
.sidebar-right {
  position: absolute;
  right: -318px;
  width: 320px;
  height: 100%;
  background-color: #2F547E;
  transition: 0.2s ease-in-out;

  &:hover {
    right: 0;
  }

  &__info {
  }
}
</style>
