<template>
  <div :class="['picto-btn relative rounded-full w-20 mr-4', color]">
    <div :class="['icon-wrap w-20 h-20', cls]" v-html="icon"></div>
  </div>
</template>

<script>
export default {
  name: 'PictoBtn',
  props: {
    color: {
      type: String,
      required: true,
    },
    icon: {
      type: String,
      required: true,
    },
    cls: {
      type: String,
      required: false,
    },
  },
};
</script>

<style scoped></style>
