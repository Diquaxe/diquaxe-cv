<template>
  <header class="header">
    <NuxtLink
      to="/"
      class="link"
      >Главная страница</NuxtLink
    >
    <nav class="nav">
      <NuxtLink
        v-for="item in links"
        :key="item.label"
        :to="item.link"
        class="link"
        >{{ item.label }}</NuxtLink
      >
    </nav>
  </header>
</template>

<script lang="ts" setup>
const links = ref([
  {
    link: "/about",
    label: "Обо мне",
  },
  {
    link: "/projects",
    label: "Проекты",
  },
  {
    link: "/contacts",
    label: "Контакты",
  },
])
</script>

<style lang="scss" scoped>
.header {
  display: flex;
  gap: 32px;
  justify-content: space-between;
  height: 64px;
  padding: 19px 24px;
  border-bottom: 1px solid $c-dt-white-100;

  @include font-body1-18-400;

  .nav {
    display: flex;
    gap: 32px;
    width: 50%;
  }

  .link {
    color: $c-dt-white-500;

    @include transition("color");

    @include hover {
      color: $c-dt-white-1000;
    }
  }
}
</style>
