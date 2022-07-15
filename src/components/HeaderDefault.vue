<script setup lang="ts">
import IconTwitterVue from './icons/IconTwitter.vue'
import IconDiscordVue from './icons/IconDiscord.vue'
</script>

<template>
  <header>
    <div class="left">
      <div @click="$router.push({ name: 'landing' })" class="logo">VIBEZ.</div>
    </div>
    <div class="right">
      <div class="button" @click="$router.push({ name: 'zone' })">The Zone</div>
      <div class="icon">
        <IconTwitterVue />
      </div>
      <div class="icon">
        <IconDiscordVue />
      </div>
    </div>
  </header>
</template>

<style lang="scss" scoped>
header {
  width: 100vw;
  display: flex;
  justify-content: space-between;
  padding: 10px var(--side-padding);
  background-color: var(--color-background);
  z-index: 10;
  &,
  .left,
  .right {
    display: flex;
    flex-direction: row;
    align-items: center;
    font-size: 26px;
    div {
      line-height: 48px;
      &:not(:last-child) {
        margin-right: 20px;
      }
      .logo {
        cursor: pointer;
        transition: color 0.2s ease;
        &:hover {
          color: black;
        }
      }
      .icon {
        cursor: pointer;
        padding-top: 4px;
        svg {
          width: 24px;
          height: 24px;
          fill: var(--sol-grey-dark);
          transition: fill 0.2s ease;
        }
        &:hover svg {
          fill: black;
        }
      }
    }
  }
  .button {
    background-color: var(--sol-grey-light);
    padding: 0 8px;
    border-radius: 14px;
    cursor: pointer;
    transition: color 0.2s ease;
    transition: background-color 0.2s ease;
    &:hover {
      color: black;
      background-color: var(--sol-grey-dark);
    }
  }
}

@media (max-width: 1024px) {
  header {
    padding: 8px var(--side-padding-mobile);
    &,
    .left,
    .right {
      font-size: 22px;
    }
  }
}
</style>
