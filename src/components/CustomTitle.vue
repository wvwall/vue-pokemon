<template>
    <div>
        <h1>{{ titleText }}</h1>
        <h2>{{ subtitleText }}</h2>
    </div>
</template>

<script>
export default {
    name: 'CustomTitle',
    props: ['titleText', 'subtitleText']
}
</script>

<style scoped>
h1 {
    color: #F7C408;
}
</style>
