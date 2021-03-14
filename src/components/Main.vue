<template>
    <main class="main">
      <SidebarLeft></SidebarLeft>

      <section class="main__content"></section>

      <SidebarRight></SidebarRight>
    </main>
</template>

<script>
import SidebarLeft from '@/components/SidebarLeft'
import SidebarRight from '@/components/SidebarRight'

export default {
  name: 'Main',
  components: {
    SidebarLeft,
    SidebarRight
  }
}
</script>

<style lang="scss">
.main {
  display: flex;
  justify-content: space-between;
  flex-grow: 1;
  flex-shrink: 0;
  height: auto;
  background-color: #3C6697;
}
</style>
