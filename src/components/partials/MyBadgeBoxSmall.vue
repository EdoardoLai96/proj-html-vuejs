<template>
    <div class="badge-box-ver_small">
        <div class="badge-icon bg-white">
            <img :src="badgeBoxSmall.url">
        </div>
        <div class="badge-text">
            <h4 class="badge-title my-3 fw-light">{{badgeBoxSmall.title}}</h4>
            <p class="badge-caption text-secondary">{{badgeBoxSmall.text}} </p>
        </div>
    </div>
</template>

<script>
export default {
    name: "MyBadgeBoxSmall",
    props: {
        badgeBoxSmall: Object,
    }

}
</script>

<style scoped lang="scss">
@import '../../assets/style/variables.scss';


</style>