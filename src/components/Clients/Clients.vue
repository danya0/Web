<template>
  <div class="w-full">
    <div class="font-['Roboto'] text-[#424242] text-[19px] leading-[22px] font-bold mb-2">
      Клиенты
    </div>
    <ClientCard
      v-for="i in 5"
      :key="i"
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
  data () {
    return {
      client: {
        name: 'Кто-то там',
        img: 'https://s3.us-west-2.amazonaws.com/images.unsplash.com/small/reserve/D9xlw7UxTBqQw5sLf8cJ_reef_insp-72.jpg',
        email: 'sobaka@mail.ru',
        phone: '88005553535'
      }
    }
  }
}
</script>
<style scoped></style>
