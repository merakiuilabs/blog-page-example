<template>
    <nav class="flex justify-center bg-white px-6 py-4 shadow">
        <div class="flex flex-col container md:flex-row md:items-center md:justify-between">
            <div class="flex justify-between items-center">
            <div>
                <a class="text-gray-800 text-2xl font-bold md:text-3xl" href="#">Brand</a>
            </div>
            <div>
                <button type="button" @click="isOpen = !isOpen" class="block text-gray-800 hover:text-gray-600 focus:text-gray-600 focus:outline-none md:hidden">
                    <svg class="h-6 w-6 fill-current" viewBox="0 0 24 24">
                        <path d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z"/>
                    </svg>
                </button>
            </div>
        </div>
        <div class="flex flex-col md:flex-row" :class="isOpen ? 'block' : ['hidden' , 'md:block']">
            <a class="my-1 text-gray-800 border-b-4 border-transparent hover:border-gray-700 hover:font-bold md:mx-4 md:my-0" href="#">Home</a>
            <a class="my-1 text-gray-800 border-b-4 border-transparent hover:border-gray-700 hover:font-bold md:mx-4 md:my-0" href="#">Blog</a>
            <a class="my-1 text-gray-800 border-b-4 border-transparent hover:border-gray-700 hover:font-bold md:mx-4 md:my-0" href="#">About us</a>
        </div>
        </div>
    </nav>
</template>

<script>
    export default {
        data() {
            return {
                isOpen: false
            }
        }
    }
</script>