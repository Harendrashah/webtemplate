<script setup>
    import FooterPage from "~/components/AppNav/FooterPage.vue";
    import NavBar from "~/components/AppNav/NavBar.vue";
</script>

<template>

    <NavBar/>
    <slot/>
    <FooterPage/>

</template>