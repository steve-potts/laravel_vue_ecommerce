

<template>

    <div class="w-[200px] bg-indigo-700 text-gray-300 py-4 px-2">
        <router-link
            :to="{name: 'app.dashboard'}"
            class="flex items-center transition-colors
                        py-1 px-2 rounded hover:bg-black/30 mb-2"
        >
            <span class="mr-2 text-gray-300">
                <HomeIcon class="w-5"/>
            </span>
            <span class="text-sm font-light">
                Dashboard
            </span>
        </router-link>
        <router-link
            :to="{name: 'app.dashboard'}"
            class="flex items-center transition-colors
                        py-1 px-2 rounded hover:bg-black/30 mb-2"
        >
            <span class="mr-2 text-gray-300">
                <ViewListIcon class="w-5"/>
            </span>
            <span class="text-sm font-light">
                Products
            </span>
        </router-link>
        <router-link
            :to="{name: 'app.dashboard'}"
            class="flex items-center transition-colors
                        py-1 px-2 rounded hover:bg-black/30 mb-2"
        >
            <span class="mr-2 text-gray-300">
                <UsersIcon class="w-5"/>
            </span>
            <span class="text-sm font-light">
                Users
            </span>
        </router-link>
        <router-link
            :to="{name: 'app.dashboard'}"
            class="flex items-center transition-colors
                        py-1 px-2 rounded hover:bg-black/30"
        >
            <span class="mr-2 text-gray-300">
                <ChartBarIcon class="w-5"/>
            </span>
            <span class="text-sm font-light">
                Reports
            </span>
        </router-link>
    </div>
</template>

<script setup>
    import { HomeIcon, UsersIcon, ViewListIcon, ChartBarIcon} from "@heroicons/vue/outline";
</script>

<style scoped>

</style>
