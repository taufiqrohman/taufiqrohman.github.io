<template>
    <div class="container mx-auto mb-4">
        <h1 :class="`text-${color}-800 font-bold text-4xl mb-0 pb-0`">{{title}}</h1>
        <h3 v-if="subtitle != null" :class="`text-lg text-${color}-900`">{{subtitle}}</h3>
    </div>
</template>

<script>

export default {
    name: "AppTitle",
    props: {
        title: String,
        subtitle: {
            type: String,
            default: null
        },
        color: {
            type: String,
            default: "indigo"
        }
    }
}
</script>