<template>
    <div class="badge-box-ver">
        <div class="badge-icon" :class="'bg-' + badgeBox.background">
            <img :src="badgeBox.url">
        </div>
        <div class="badge-text">
            <h4 class="badge-title  my-3">{{badgeBox.title}}</h4>
            <p class="badge-caption text-secondary">{{badgeBox.text}} </p>
        </div>
    </div>
</template>

<script>
export default {
    name: "MyBadgeBox",
    props: {
        badgeBox: Object,
    }

}
</script>

<style scoped lang="scss">
@import '../../assets/style/variables.scss';


</style>