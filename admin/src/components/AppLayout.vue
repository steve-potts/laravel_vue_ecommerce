

<template>
    <div class="flex min-h-full bg-gray-100">
        <Sidebar :class="{'-ml-[200px]': !sidebarOpened}"></Sidebar>
        <div class="flex-1">
            <TopHeader @toggle-sidebar="toggleSidebar"/>
            <main class="p-6">
                <div class="p-4 rounded bg-white">
                    <router-view></router-view>
                </div>
            </main>
        </div>
    </div>
</template>

<script setup>
    import {ref, onMounted, onUnmounted} from 'vue';
    import Sidebar from "./Sidebar.vue";
    import TopHeader from "./TopHeader.vue";

    const { title } = defineProps({
        title: String
    })

    const sidebarOpened = ref(true);

    function toggleSidebar() {
        sidebarOpened.value = !sidebarOpened.value;
    }

    onMounted(() => {
        handleSidebarOpened();
        window.addEventListener('resize', handleSidebarOpened);
    })

    onUnmounted(() => {
        window.removeEventListener('resize', handleSidebarOpened);
    })

    function handleSidebarOpened() {
        sidebarOpened.value = window.outerWidth > 768;

    }

</script>

<style scoped>

</style>
