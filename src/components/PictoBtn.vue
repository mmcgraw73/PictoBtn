<template>
  <div class="main-wrap relative w-20 h-20 rounded-full bg-blue-200">
    
  </div>
</template>

<script>
export default {
  name: 'PictoBtn',
  props: {
    bg_color: {
      type: String,
      required: true,
    },
    icon: {
      type: String,
      required: true,
    },
  },
  data() {
    return {};
  },
};
</script>

<style scoped></style>
