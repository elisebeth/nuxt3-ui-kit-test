<script setup lang="ts">
import { useI18n } from 'vue-i18n'

import Button from './components/Button/Button.vue'

const i18n = useI18n()

console.log(i18n.t('test-message'))

i18n.locale.value = 'en'

console.log(i18n.t('test-message'))
</script>

<template>
  <main>
    main
    <Button :mode="'large'"/>
  </main>
</template>

<style scoped></style>
