<template>
  <div :class="['picto-btn grid grid-cols-2 gap-2 cursor-pointer']">
    <div
      :class="['icon-wrap w-20 h-20 rounded-full', cls, color]"
      v-html="icon"
    ></div>
    <p class="text-xs font-bold pt-5">{{ details }}</p>
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
    details: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped></style>
