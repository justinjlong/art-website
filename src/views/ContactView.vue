<template>
  <div class="contact">
    <p>{{ email }}</p>
  </div>
</template>

<script lang="ts">
export default {
  data() {
      return {
         email: "justinjlongart@gmail.com"
      }
    }
}
</script>

<style>
@media (min-width: 1024px) {
  .contact {
    min-height: 80vh;
    display: flex;
    align-items: center;
    flex-direction: column !important;
    justify-content: center;
  }
}
</style>
