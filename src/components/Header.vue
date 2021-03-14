<template>
    <header class="header">
      <div class="header__wrapper">
        <div class="header__content">
          <button class="header__burger">
            <svg class="icon-menu"
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg">

              <path class="icon-menu__top-element"
                d="M1.5 6.5C0.671573 6.5 0 5.82843 0 5C0 4.17157 0.671573 3.5 1.5
                3.5H22.5C23.3284 3.5 24 4.17157 24 5C24 5.82843 23.3284 6.5 22.5 6.5H1.5Z"
                fill="white"/>

              <path class="icon-menu__middle-element"
                d="M0 12C0 12.8284 0.671573 13.5 1.5 13.5H22.5C23.3284 13.5 24 12.8284
                24 12C24 11.1716 23.3284 10.5 22.5 10.5H1.5C0.671573 10.5 0 11.1716 0 12Z"
               fill="white"/>

              <path class="icon-menu__bottom-element"
                d="M0 19C0 19.8284 0.671573 20.5 1.5 20.5H22.5C23.3284 20.5 24 19.8284
                24 19C24 18.1716 23.3284 17.5 22.5 17.5H1.5C0.671573 17.5 0 18.1716 0 19Z"
                fill="white"/>
            </svg>
          </button>

          <a class="header__logo" href="/">
            .codebook
          </a>

          <button class="header__search">
            <svg class="icon-search"
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg">
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M15.7399 13.6961C18.1533 10.3096 17.8409 5.5779 14.8028 2.53975C11.4164 -0.846584 5.92608
                -0.846583 2.53975 2.53975C-0.846584 5.92608 -0.846584 11.4164 2.53975 14.8028C5.5779 17.8409
                10.3096 18.1533 13.6961 15.7399L21.9562 24L24 21.9562L15.7399 13.6961ZM12.7589 4.58358C15.0165
                6.84114 15.0165 10.5014 12.7589 12.7589C10.5014 15.0165 6.84114 15.0165 4.58358 12.7589C2.32603
                10.5014 2.32603 6.84114 4.58358 4.58358C6.84114 2.32603 10.5014 2.32603 12.7589 4.58358Z"
                fill="white"/>
            </svg>
          </button>
        </div>
      </div>
    </header>
</template>

<script>
export default {
  name: 'Header',
  components: {}
}
</script>

<style lang="scss">
.header {
  position: sticky;
  top: 0;
  flex-grow: 0;
  flex-shrink: 0;
  height: 48px;
  background-color: #2F547E;
  @media (min-width: 1280px) {
    height: 60px;
  }

  &__wrapper {
    height: 100%;
    padding: 0 10px;
    @media (min-width: 768px) {
      padding: 0 20px;
    }
  }

  &__content {
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: 100%;
  }

  &__burger {
  }

  &__logo {
    font-size: 24px;
    line-height: 100%;
    text-decoration: none;
  }

  &__search {
  }
}

.icon-menu {
  &:hover {
    .icon-menu__top-element {
      transform: translateY(-3px);
    }

    .icon-menu__middle-element {}

    .icon-menu__bottom-element {
      transform: translateY(3px);
    }
  }

  &__top-element {
    transition: 0.2s ease-in-out;
    transform: translateY(0);
  }

  &__middle-element {
    transition: 0.2s ease-in-out;
  }

  &__bottom-element {
    transition: 0.2s ease-in-out;
    transform: translateY(0);
  }
}

.icon-search {
  transform: scale(1);
  transition: 0.2s ease-in-out;
  &:hover {
    transform: scale(1.15);
  }
}

</style>
