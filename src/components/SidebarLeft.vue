<template>
    <aside class="sidebar-left">
      <i class="sidebar-left__info">SidebarLeft</i>
    </aside>
</template>

<script>
export default {
  name: 'SidebarLeft',
  components: {}
}
</script>

<style lang="scss">
.sidebar-left {
  position: absolute;
  left: -318px;
  width: 320px;
  height: 100%;
  background-color: #2F547E;
  transition: 0.2s ease-in-out;

  &:hover {
    left: 0;
  }

  &__info {
  }
}
</style>
