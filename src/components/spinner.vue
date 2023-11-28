<script>
export default {
    name: 'spinner'
}
</script>

<template>
    <div class="spin">
        <div class="spinner-border text-success fs-6" role="status">
        <span class="visually-hidden">Loading...</span>
    </div>
</div>
</template>

<style scoped lang="scss">
    .spin{
        text-align: center;
        padding-top: 50px;
    }
</style>