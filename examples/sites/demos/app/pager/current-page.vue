<template>
  <tiny-pager layout="prev, pager, next" :current-page="2" :total="50"></tiny-pager>
</template>

<script lang="jsx">
import { Pager } from '@opentiny/vue'

export default {
  components: {
    TinyPager: Pager
  }
}
</script>
