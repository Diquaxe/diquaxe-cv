<template>
  <div class="index-project">
    <div class="sidebar">
      <div class="title">Никита Мохов</div>
      <div class="subtitle">UX UI дизайнер</div>
      <div class="text">
        Привет! Я UX UI дизайнер в BuroBuro. Работаю с B2C и B2B проектами и
        нагруженными интерфейсами. Ценю работу в команде и всегда стремлюсь к
        прокачке собственных скиллов.
      </div>
    </div>
    <div class="content">
      <IndexProject />
    </div>
  </div>
</template>

<script lang="ts" setup></script>

<style lang="scss" scoped>
.sidebar {
  .title {
    @include font-subheadline-20-500;
  }
}
</style>
