<template>
    <Home />
</template>

<script>
export default {
    layout: 'default',
    methods: {
        login() {
            navigateTo('/login')
        }
    }
}
</script>