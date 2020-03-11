<template>
  <div id="hc-main" class="d-flex flex-column" :class="{ conditionalClass: true }">
    <router-view :key="$route.fullPath"></router-view>
  </div>
</template>

<script>
import storeMixin from '@/demo/store/mixins'
import DemoOptions from './components/DemoOptions'

export default {
  mixins: [storeMixin],

  components: { DemoOptions }
}
</script>
