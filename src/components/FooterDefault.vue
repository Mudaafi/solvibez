<script setup lang="ts">
import IconTwitter from './icons/IconTwitter.vue'
import IconDiscord from './icons/IconDiscord.vue'
</script>

<template>
  <footer>
    <div class="left"></div>
    <div class="right">
      <div class="button" @click="$router.push({ name: 'zone' })">The Zone</div>
      <div class="icon">
        <IconTwitter />
      </div>
      <div class="icon">
        <IconDiscord />
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
footer {
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
  footer {
    padding: 8px var(--side-padding-mobile);
    justify-content: center;
    &,
    .left,
    .right {
      font-size: 22px;
    }
  }
}
</style>
