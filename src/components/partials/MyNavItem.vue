<template>
        <a :href="nav_item.href" class="nav-item seco mx-2 py-2 px-3 text-center">
          <i class="fs-4"  :class="nav_item.icon_name"></i>
          <p class="text-center mb-0">{{nav_item.text}}</p>
        </a>

</template>

<script>
export default {
    name: "MyNavItem",
    props: {
        nav_item: Object
    }

}
</script>

<style lang="scss" scoped>
 @import "../../assets/style/variables.scss";

  .nav-item{
    text-decoration: none;
    &:hover{
      background-color: $primaryColor;
      color: white;
      cursor: pointer;
      transition: background-color 0.4s;
    }
    .nav_icon{
      transform: scale(0.8);
    }
  }

</style>