<script setup>
import TheWelcome from '@/components/TheWelcome.vue'
import DefaultLayout from '@/layouts/Default.vue'
</script>

<template>
  <DefaultLayout>
    <main>
      <TheWelcome/>
    </main>
  </DefaultLayout>
</template>

<script>
export default {
  created() {
    this.axios.get('https://yandex.ru').then(response => {
      console.log(response);
    });
  },
}
</script>
