<template>
  <div class="events">
    <EventList v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
// @ is an alias to /src

import EventList from "@/components/EventList.vue"

export default {
  name: "HomeView",
  components: {
    EventList,
  },
  data() {
    return {
      events: [
        {
          id: 15487,
          time: "12:00",
          date: "Juan 28,2022",
          title: "Learn Angular",
          description: "Lorem ipsum dolor sit amet consectetur.",
        },
        {
          id: 51458,
          time: "15:00",
          date: "Juan 15,2022",
          title: "Learn Vue Js",
          description: "Lorem ipsum dolor sit amet consectetur.",
        },
      ],
    }
  },
}
</script>

<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
