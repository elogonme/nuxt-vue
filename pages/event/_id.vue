<template>
  <div>
    <h1>Event #{{ this.$route.params.id }}</h1>
  </div>
</template>
<script>
export default {
  head() {
    return {
      title: 'Event - #' + this.id,
      meta: [
        {
          hid: 'discription',
          name: 'descrition',
          content: 'What you need to know about Event #' + this.id,
        },
      ],
    }
  },
  computed: {
    id() {
      return this.$route.params.id
    },
  },
}
</script>
