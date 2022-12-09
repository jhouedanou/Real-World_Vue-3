<template>
  <div class="events">
    <h1>Events For Good</h1>
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
  import axios from 'axios'

// @ is an alias to /src
import EventCard from '@/components/EventCard.vue'
export default {
  name: 'Home',
  components: {
    EventCard
  },
  data() {
    return {
      events: null
    }
  },
  created(){

  }
}
</script>

<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
