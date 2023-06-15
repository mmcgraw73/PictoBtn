<template>
  <div class="main-wrap flex items-center">
    <PictoBtn :color="'bg-red-500'" :cls="'pl-7 pt-6'" :icon="icons.exclamation_bulb" />
    <PictoBtn :color="'bg-green-500'" :cls="'pl-7 pt-6'" :icon="icons.ghost" />
    <PictoBtn :color="'bg-red-500'" :cls="'pl-5 pt-6'" :icon="icons.hand_dollar" />
    <PictoBtn :color="'bg-red-500'" :cls="'pl-6 pt-6'" :icon="icons.user_plus" />
    <PictoBtn :color="'bg-green-500'" :cls="'pl-6 pt-6'" :icon="icons.user_check" />
    <PictoBtn :color="'bg-red-500'" :cls="'pl-5 pt-6'" :icon="icons.hand_dollar" />
  </div>
</template>

<script>
import icons from '../../assets/icons';
import PictoBtn from './PictoBtn';
export default {
  name: 'ExecutiveSummary',
  components: {
    PictoBtn,
  },
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
    return {
      ...icons,
      color: '',
    };
  },
};
</script>

<style scoped
.main-wrap {
  width: 400px
}
</style>
