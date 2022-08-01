<template>
  <div class="w-full">
    <div class="font-['Roboto'] text-[#424242] text-[19px] leading-[22px] font-bold mb-2">
      Клиенты
    </div>
    <ClientCard
      v-for="client in clients"
      :key="client.uid"
      class="mb-2"
      :client="client"
    />
    <ListBlocAdd class="mt-2" />
  </div>
</template>
<script>
import ClientCard from '@/components/Clients/ClientCard.vue'
import ListBlocAdd from '@/components/Common/ListBlocAdd.vue'

export default {
  components: {
    ClientCard,
    ListBlocAdd
  },
  computed: {
    clients () {
      return this.$store.state.clients.clients
    }
  }
}
</script>
<style scoped></style>
