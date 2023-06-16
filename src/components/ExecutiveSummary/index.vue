<template>
  <div
    class="
      main-wrap
      grid grid-cols-5
      bg-gray-700
      p-3
      gap-2
      rounded
      items-center
    "
  >
    <PictoBtn
      :color="'bg-red-500'"
      :cls="''"
      :icon="icons.user_minus"
      :details="`${user_minus.response} ${user_minus.static} `"
    />
    <PictoBtn
      :color="'bg-red-500'"
      :cls="''"
      :icon="icons.hand_dollar"
      :details="`$${hand_dollar.response} ${hand_dollar.static} `"
    />
    <PictoBtn
      :color="'bg-green-500'"
      :cls="''"
      :icon="icons.users_rectangle"
      :details="`${users_rectangle.response} ${users_rectangle.static} `"
    />
    <PictoBtn
      :color="'bg-blue-500'"
      :cls="''"
      :icon="icons.follow_up"
      :details="`${follow_up.response}% ${follow_up.static}`"
    />
    <PictoBtn
      :color="'bg-green-500'"
      :cls="''"
      :icon="icons.users_add"
      :details="`${users_add.response} ${users_add.static} `"
    />
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
  data() {
    return {
      ...icons,
      user_minus: {
        static: 'Customers at risk',
        response: '47767', // this value will be a computed prop that returns the response value once endpoints are in place
      },
      hand_dollar: {
        static: 'Royalties at risk',
        response: '777767', // this value will be a computed prop that returns the response value once endpoints are in place
      },
      users_rectangle: {
        static: 'Customers retained',
        response: '744', // this value will be a computed prop that returns the response value once endpoints are in place
      },
      follow_up: {
        static: 'Follow up rate',
        response: '13', // this value will be a computed prop that returns the response value once endpoints are in place
      },
      users_add: {
        static: 'Customers acquired',
        response: '28', // this value will be a computed prop that returns the response value once endpoints are in place
      },
    };
  },
};
</script>

<style scoped>
.main-wrap {
  width: 750px;
  height: 100px;
}
svg {
  display: block;
  margin: auto;
}
</style>
