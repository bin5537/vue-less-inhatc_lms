<script setup>
    import Header from "./components/Header.vue";
    import Banner from "./components/Banner.vue";
    import SideBar from "./components/Sidebar.vue";
    import Content from "./components/Content.vue";
    import Footer from "./components/Footer.vue";
    
    import '@fortawesome/fontawesome-free/css/all.min.css';
</script>

<template>

    <Header />
    <Banner />
    <SideBar />
    <Content />
    <Footer />

</template>

<style lang="less">
    @import url("../src/assets/style.less");
    @import url("../src/assets/style-Header.less");
    @import url("../src/assets/style-Banner.less");
    @import url("../src/assets/style-Sidebar.less");
    @import url("../src/assets/style-Content.less");
    @import url("../src/assets/style-Footer.less");
</style>