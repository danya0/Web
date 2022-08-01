<template>
  <div class="w-full">
    <ClientCard
      :employee="employee"
    />
  </div>
</template>
<script>
import ClientCard from '@/components/Clients/ClientCard'

export default {
  components: {
    ClientCard
  },
  data () {
    return {
      employee: {
        name: 'Кто-то там',
        img: 'https://s3.us-west-2.amazonaws.com/images.unsplash.com/small/reserve/D9xlw7UxTBqQw5sLf8cJ_reef_insp-72.jpg'
      }
    }
  }
}
</script>
<style scoped></style>
