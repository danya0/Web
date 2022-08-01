<template>
  <ListBlocItem
    :title="employee.name"
  >
    <img
      class="w-[20px] h-[20px] rounded"
      :src="employee.img"
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
    employee: {
      type: Object,
      default: () => ({})
    }
  }
}
</script>

<style>

</style>
