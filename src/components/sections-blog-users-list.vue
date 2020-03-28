<template>
    <div class="flex flex-col bg-white max-w-sm px-6 py-4 mx-auto rounded-lg shadow-md">
        <ul class="-mx-4">
            <li class="flex items-center">
                <img class="w-10 h-10 object-cover rounded-full mx-4" src="https://images.unsplash.com/photo-1492562080023-ab3db95bfbce?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=731&q=80" alt="avatar">
                <p>
                    <a class="text-gray-700 font-bold mx-1 hover:underline" href="#">Alex John</a>
                    <span class="text-gray-700 text-sm font-light">Created 23 Posts</span>
                </p>
            </li>

            <li class="flex items-center mt-6">
                <img class="w-10 h-10 object-cover rounded-full mx-4" src="https://images.unsplash.com/photo-1464863979621-258859e62245?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=333&q=80" alt="avatar">
                <p>
                    <a class="text-gray-700 font-bold mx-1 hover:underline" href="#">Jane Doe</a>
                    <span class="text-gray-700 text-sm font-light">Created 52 Posts</span>
                </p>
            </li>
            
            <li class="flex items-center mt-6">
                <img class="w-10 h-10 object-cover rounded-full mx-4" src="https://images.unsplash.com/photo-1531251445707-1f000e1e87d0?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=281&q=80" alt="avatar">
                <p>
                    <a class="text-gray-700 font-bold mx-1 hover:underline" href="#">Lisa Way</a>
                    <span class="text-gray-700 text-sm font-light">Created 73 Posts</span>
                </p>
            </li>

            <li class="flex items-center mt-6">
                <img class="w-10 h-10 object-cover rounded-full mx-4" src="https://images.unsplash.com/photo-1500757810556-5d600d9b737d?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=735&q=80" alt="avatar">
                <p>
                    <a class="text-gray-700 font-bold mx-1 hover:underline" href="#">Steve Matt</a>
                    <span class="text-gray-700 text-sm font-light">Created 245 Posts</span>
                </p>
            </li>

            <li class="flex items-center mt-6">
                <img class="w-10 h-10 object-cover rounded-full mx-4" src="https://images.unsplash.com/photo-1502980426475-b83966705988?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=373&q=80" alt="avatar">
                <p>
                    <a class="text-gray-700 font-bold mx-1 hover:underline" href="#">Khatab Wedaa</a>
                    <span class="text-gray-700 text-sm font-light">Created 332 Posts</span>
                </p>
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
        props: ['data']
    }
</script>