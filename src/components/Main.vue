<template>
    <main class="main-page">
      <SidebarLeft></SidebarLeft>

      <section class="main-page__content container">
        <h1 class="main-page__title">Справочник веб-разработчика</h1>

        <ul class="main-page__tech-list">
          <li class="main-page__tech-item">
            <svg class="main-page__icon"
              width="75"
              height="90"
              viewBox="0 0 75 90"
              fill="none"
              xmlns="http://www.w3.org/2000/svg">
              <path
                d="M0 0H75L68.1766 80.8578L37.4166 90L6.83292 80.8578L0 0ZM25.1097
                36.5587L24.2848 26.3702L60.2041 26.3802L61.029 16.5521L13.9662 16.5421L16.4553
                46.5721H49.0463L47.8877 59.4192L37.4976 62.4332L26.9407 59.4042L26.2684 51.4937H16.9512L18.1289
                67.1295L37.4976 72.5668L56.7042 67.1595L59.3649 36.5637H25.1097V36.5587Z"
                fill="white"/>
            </svg>

            <h2 class="main-page__tech-name">HTML</h2>
          </li>

          <li class="main-page__tech-item">
            <svg class="main-page__icon"
              width="75"
              height="90"
              viewBox="0 0 75 90"
              fill="none"
              xmlns="http://www.w3.org/2000/svg">
              <path
                d="M0 0H75L68.1796 80.8618L37.4207 90L6.82997 80.8568L0 0ZM61.0375 16.5466L13.9673 16.5365L14.7262
                26.3656L50.8886 26.3757L49.9808 36.5628H26.2632L27.123 46.2104H49.2027L47.8963 59.4234L37.5024
                62.4392L26.9501 59.3982L26.2728 51.4855H16.9549L17.9923 65.9442L37.5024 72.3238L56.6907
                66.5897L61.0375 16.5466Z"
                fill="white"/>
            </svg>

            <h2 class="main-page__tech-name">CSS</h2>
          </li>

          <li class="main-page__tech-item">
            <svg class="main-page__icon"
              width="75"
              height="90"
              viewBox="0 0 75 90"
              fill="none"
              xmlns="http://www.w3.org/2000/svg">
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M0 0L6.96178 80.9197L37.4415 90L68.0967 80.8579L75 0.0308849L0 0ZM27.2328
                17.3576H34.6919V70.4187L12.695 64.1489L12.6658 54.6671L27.1451 58.8367L27.2328
                17.3576ZM62.8811 38.9723L60.8594 64.9062L40.6132 70.47L40.4667 61.0733L55.1166
                56.9622L55.3217 49.2964L40.789 51.9238L40.4667 17.4896L64.5219 17.3659L63.8773
                26.8245L47.9382 26.8863V40.7342L62.8811 38.9723Z"
                fill="white"/>
            </svg>

            <h2 class="main-page__tech-name">JavaScript</h2>
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
.main-page {
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

  &__title {}

  &__tech-list {
    display: block;
  }

  &__tech-item {
    display: block;
  }

  &__tech-name {}
}
</style>
