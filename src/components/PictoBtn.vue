<template>
  <div class="main-wrap relative w-20 border-radius-full">
    <h1 class="mx-auto mt-5 bg-blue-200">Tailwind Start</h1>
  </div>
</template>

<script>
export default {
  name: 'PictoBtn',
  props: {
    bg_color: {
      type: String,
      required: true
    },
    icon: {
      type: String,
      required: true
    }
  },
  data() {
    return {};
  },
};
</script>

<style scoped></style>
