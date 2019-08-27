<template>
  <div >
    <BurgerMenu></BurgerMenu>
        <nuxt />
  </div>
</template>

<script>
import BurgerMenu from '~/components/UI/BurgerMenu.vue'
export default{
  components:{
    BurgerMenu
  }
}
</script>
