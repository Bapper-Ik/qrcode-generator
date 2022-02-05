<template>
    <Generate v-on:qr-text="displayOutput" />
    <div class="output mt-20 py-6 flex justify-center invisible mb-36">
        <img id="myImg" src="" alt="">
    </div>
</template>


<script>
import Generate from "./Generate";

export default {
    name: 'Output',
    components: {
        Generate,
    },

    methods: {
        displayOutput(qrText) {
            document.querySelector('#myImg').src = `https://api.qrserver.com/v1/create-qr-code/?size=150x150&data=${qrText}`

            document.querySelector('.output').style.visibility = 'visible'
        }
    }
}
</script>
