<template>
    <Generate v-on:qr-text="displayOutput" />
    <div class="output grid grid-col-2 gap-4 mt-20 py-6 flex justify-center mb-36 invisible">
        <img class="" id="myImg" src="" alt="" />
        <div class="bg-green-400 my-4 py-2 px-8 text-white rounded-lg">
            <button class="" @click="onClick">Download</button>
        </div>
        
    </div>
</template>


<script>
import Generate from "./Generate";
import axios from "axios";

export default {
    name: 'Output',
    components: {
        Generate,
    },

    methods: {
        displayOutput(qrText) {
            document.querySelector('#myImg').src = `https://api.qrserver.com/v1/create-qr-code/?size=150x150&data=${qrText}`

            document.querySelector('.output').style.visibility = 'visible'
        },

         onClick(){
            axios({
                url: document.querySelector('#myImg').src,
                method: 'GET',
                responseType: 'blob'

            })
            .then((response) => {
                const fileurl = window.URL.createObjectURL(new Blob([response.data]))
                const fileLink = document.createElement('a')
                fileLink.href = fileurl
                fileLink.setAttribute('download', 'image.jpg')
                document.body.appendChild(fileLink)

                fileLink.click();
    
            })
            .catch(err => console.log(err))
        }
    }
}
</script>
