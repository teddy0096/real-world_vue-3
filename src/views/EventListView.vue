<script setup>
import EventCard from '@/components/EventCard.vue'
import { ref } from 'vue'

const events = ref([
  {
    id: 5928101,
    category: 'animal welfare',
    title: 'Cat adoption Day',
    description: 'Find your new feline friend at this event',
    location: 'Meow Town',
    date: 'January 28, 2022',
    time: '12: 00',
    petsAllowed: true,
    organization: 'Kat Laydee'
  },
  {
    id: 1328101,
    category: 'animal welfare',
    title: 'Dog adoption Day',
    description: 'Find your new feline friend at this event',
    location: 'Meow Town',
    date: 'January 28, 2022',
    time: '12: 00',
    petsAllowed: true,
    organization: 'Kat Laydee'
  },
  {
    id: 5923401,
    category: 'animal welfare',
    title: 'Bird adoption Day',
    description: 'Find your new feline friend at this event',
    location: 'Meow Town',
    date: 'January 28, 2022',
    time: '12: 00',
    petsAllowed: true,
    organization: 'Kat Laydee'
  }
])
</script>

<template>
  <h1>Events For Good</h1>
  <div class="events">
    <EventCard v-for="event in events" :key="events.id" :event="event" />
  </div>
</template>

<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
