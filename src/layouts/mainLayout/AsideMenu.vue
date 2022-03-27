<template>
  <div class="aside">
    <nav class="aside-menu">
      <div class="logo" />
      123
    </nav>
  </div>
</template>
<style>
@import "../../assets/root.css";

.aside {
  background-color: var(--background-color__aside-menu);
}
.aside-menu {
  display: flex;
  flex-direction: column;
  align-items: center;
  color: var(--font-color__aside-menu);
  min-height: 100vh;
  width: var(--aside-width);
}
.logo {
  padding-top: 20px;
  display: block;
  width: 4rem;
  height: 4rem;
  background-image: var(--aside-logo-background-image);
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
}
</style>
