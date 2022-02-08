<template>
    <div class="bg-gray-600 max-w-full py-4 md:flex">
        <div class="py-2 md:px-5 md:flex-auto">
            <h1 class="text-white font-bold text-xl font-medium md:text-left">QR-Code Generator</h1> 
        </div>
        
        <div class="font-bold text-white py-2 md:py-2 md:py-0 md:flex-auto">
            <router-link to="/">Home</router-link> |
            <router-link to="/about">About</router-link> |
            <router-link to="/usage">Tips</router-link>
        </div>
        
    </div>
</template>


<script>

export default {
    name: 'Header',
}
</script>