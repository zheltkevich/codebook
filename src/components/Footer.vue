<template>
    <footer class="footer">
      <i class="footer__copyright">© Copyright 2021</i>
    </footer>
</template>

<script>
export default {
  name: 'Footer',
  components: {}
}
</script>

<style lang="scss">
.footer {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-grow: 0;
  flex-shrink: 0;
  height: 40px;
  background-color: #2F547E;

  &__copyright {
    font-size: 12px;
  }
}
</style>
