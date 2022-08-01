<template>
  <ListBlocItem
    :title="client.name"
    :sub-title="client.email"
  >
    <img
      class="w-[20px] h-[20px] rounded"
      :src="client.img"
    >
  </ListBlocItem>
</template>

<script>
import ListBlocItem from '@/components/Common/ListBlocItem.vue'

export default {
  components: {
    ListBlocItem
  },
  props: {
    client: {
      type: Object,
      default: () => ({})
    }
  }
}
</script>

<style>

</style>
