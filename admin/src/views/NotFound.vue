<template>
    <div class="flex min-h-full min-w-full justify-center items-center">
        <div class="text-indigo-600 text-5xl p-8 font-bold border-r pb-8">404</div>
        <div class="px-8">
            <h1 class="text-5xl font-bold mb-4">Page Not Found</h1>
            <p class="text-gray-600 text-2xl mb-4">Please check the url in address bar and try again!</p>
            <div>
                <router-link :to="{name: 'app.dashboard'}" class="flex justify-center rounded-md
                bg-indigo-600 px-3 py-1.5 text-sm font-semibold
                leading-6 text-white shadow-sm hover:bg-indigo-500
                focus-visible:outline focus-visible:outline-2
                focus-visible:outline-offset-2
                focus-visible:outline-indigo-600">
                    Go Home
                </router-link>
            </div>
        </div>
    </div>
</template>

<script setup>

</script>

<style scoped>

</style>
