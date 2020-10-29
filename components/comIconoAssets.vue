<template>
    <svg style="width: 0px; height: 0px">
        <use xmlns:xlink="http://www.w3.org/1999/xlink" :xlink:href="urlsvg"></use>
    </svg>
</template>
<script>
export default {
    name: 'com-icono-assets',
    data () {
        return {
            urlsvg: '~/assets/svg/sprite/icons.svg#i-' + this.iconName
        }
    },
    props: {
        iconName: String,
    }
}
</script>