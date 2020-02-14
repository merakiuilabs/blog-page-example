<template>
    <div class="w-32 relative">
        <select class="block appearance-none w-full bg-gray-300 text-gray-700 py-2 px-3 pr-8 rounded-lg leading-tight focus:outline-none md:px-4 md:py-3" id="grid-state">
            <option>Latest</option>
            <option>Last Week</option>
        </select>
        <div class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 text-gray-700">
            <svg class="h-6 w-6 fill-current" viewBox="0 0 30 30">
                <path d="M15 2.8125C8.26904 2.8125 2.8125 8.26904 2.8125 15C2.8125 21.731 8.26904 27.1875 15 27.1875C21.731 27.1875 27.1875 21.731 27.1875 15C27.1875 8.26904 21.731 2.8125 15 2.8125ZM15 18.75L9.375 13.125H20.625L15 18.75Z"/>
            </svg>
        </div>
    </div>
</template>


<script>
    export default {}
</script>