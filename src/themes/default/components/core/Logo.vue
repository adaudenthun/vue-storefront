<template>
  <router-link to="/" :title="$t('Home Page')" class="no-underline inline-flex">
    <img
      :width="width"
      :height="height"
      src="/assets/logo.svg"
      alt="Vuestore logo"
    >
  </router-link>
</template>

<script>
import { coreComponent } from 'lib/themes'

export default {
  props: {
    width: {
      type: [String, Number],
      required: true
    },
    height: {
      type: [String, Number],
      required: true
    }
  },
  mixins: [coreComponent('core/Logo')]
}
</script>
