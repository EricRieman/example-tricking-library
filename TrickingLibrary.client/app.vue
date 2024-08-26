<template>
  <div>
    <NuxtRouteAnnouncer />
    <NuxtWelcome />
    <q-btn color="primary" label="Primary" />
    <pre>{{ data }}</pre>
  </div>
</template>

<script setup>
  const data = await useFetch( 'https://localhost:7041/WeatherForecast' )
</script>
