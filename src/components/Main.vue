<template>
    <main class="main">
      <SidebarLeft></SidebarLeft>

      <section class="main__content container">
        <h1 class="main__title">Справочник веб-разработчика</h1>
        <ul>
          <li>
            <h2 class="main__">HTML</h2>
          </li>
          <li>
            <h2 class="main__">CSS</h2>
          </li>
          <li>
            <h2 class="main__">JavaScript</h2>
          </li>
        </ul>
      </section>

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
  position: relative;
  display: flex;
  justify-content: space-between;
  flex-grow: 1;
  flex-shrink: 0;
  height: auto;
  overflow: hidden;
  background-color: #3C6697;

  &__content {
    flex-grow: 1;
    flex-shrink: 0;
    max-width: 100%;
  }
}
</style>
