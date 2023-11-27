
<script>
export default {
    props: {
        data: Object,
    },
};
</script>

<template>
    <div class="card">
        <img :src="data.image_url" alt="">
        <h3>{{ data.name }}</h3>
        
    </div>
</template>


<style lang="scss" scoped></style>