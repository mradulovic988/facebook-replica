<template>
    <div class="flex flex-col flex-1 h-screen overflow-y-hidden">
        <Nav />

        <div class="flex overflow-y-hidden flex-1">
            <Sidebar />
            <div class="overflow-x-hidden w-2/3">
                <router-view></router-view>
            </div>
        </div>
    </div>
</template>

<script>
    import Nav from './Nav';
    import Sidebar from './Sidebar';
    export default {
        name: "App",

        components: {
            Nav,
            Sidebar
        }
    }
</script>

<style scoped>

</style>
