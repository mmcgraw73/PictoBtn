<template>
  <div class="picto-btn-wrap relative w-15 h-15">
    <div class="">
      <div :class="['picto-btn grid grid-cols-3 items-center gap-4 text-sm']">
        <div
          :class="['icon-wrap w-10 h-10 rounded-full pt-2', cls, color]"
          v-html="icon"
        ></div>
        <p class="text-xxs text-cyan-800 underline font-bold col-span-2">
          {{ details }}
        </p>
      </div>
    </div>
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

<style scoped>
.text-xxs {
  font-size: 11px;
  line-height: 15px;
}
</style>
