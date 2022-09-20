<template>
  <div>
   Kyiv Time: {{ timeData.utc_datetime }}
  </div>
</template>

<script setup>
const { data: timeData } = await useFetch('https://worldtimeapi.org/api/timezone/Europe/Kiev')
</script>
