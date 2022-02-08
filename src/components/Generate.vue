<template>
    <div class="bg-green-100 mx-auto py-4 overflow-hidden w-fit">
        <form v-on:submit="generate" class="mx-5 py-6 w-fit">
            <input class="qrText focus:outline-none rounded-xl w-full md:w-10/12 mb-4 md:mb-0 md:mr-8 p-5" type="text" name="qrText" v-model="qrText" placeholder="Type anything you want 😃">

            <input type="submit" value="Generate" v-on:click="generate" class="bg-blue-400 hover:bg-blue-500 text-white rounded-xl p-3 mr-0">
            
        </form>
    </div>
    
</template>

<script>
import '../assets/tailwind.css';

export default {
    name: 'Generate',

    data() {
        return {
            qrText: '',
        }
    },

    methods: {
        generate(e) {
            e.preventDefault()
            this.$emit('qr-text', this.qrText)
            this.qrText = ''
        },  
    }
}
</script>


