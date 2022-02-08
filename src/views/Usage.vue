<template>
    <div class="mx-5 mt-7">
        <h1 class="text-left text-2xl font-bold ">Guide</h1>
        <div class="bg-green-100 mb-12 rounded-xl py-5 md:grid md:grid-cols-3 md:gap-4">
            
            <div class="bg-white mb-10 mx-auto max-w-sm rounded-xl overflow-hidden shadow-lg">        
                <div class="px-6 py-4">
                    <div class="font-bold text-xl mb-2">Simple Text</div>
                    <p class="text-gray-700 text-base">
                    QR Code is used for welcome message at conference, auctioning meeting and other congress meetings 
                    </p>
                </div>
            </div>

            <div class="bg-white mb-10 mx-auto max-w-sm rounded-xl overflow-hidden shadow-lg">        
                <div class="px-6 py-4">
                    <div class="font-bold text-xl mb-2">Address</div>
                    <p class="text-gray-700 text-base">
                   personal home address, business address, Email Address or even personal or company's phone number
                    </p>
                </div>
            </div>

            <div class="bg-white mb-10 mx-auto max-w-sm rounded-xl overflow-hidden shadow-lg">        
                <div class="px-6 py-4">
                    <div class="font-bold text-xl mb-2">Website URLs</div>
                    <p class="text-gray-700 text-base">
                    QR Code can be used to store addresses of websites or specific web pages, and it will also be used to store urls for for some specific Application
                    </p>
                </div>
            </div>


            <div class="bg-white mb-10 mx-auto max-w-sm rounded-xl overflow-hidden shadow-lg">
                <div class="px-6 py-4">
                    <div class="font-bold text-xl mb-2">Payment</div>
                    <p class="text-gray-700 text-base">
                    QR codes can store information about your bank account or credit card, and also can be use for making transaction
                    </p>
                </div>
            </div>


            <div class="bg-white mb-10 mx-auto max-w-sm rounded-xl overflow-hidden shadow-lg">
                <div class="px-6 py-4">
                    <div class="font-bold text-xl mb-2">WiFi Authentication</div>
                    <p class="text-gray-700 text-base">
                    QR codes can be used to store WiFi networks authentication details such as SSID, password, and encryption type: when you scan such a QR code using your smartphone, it can automatically join that network
                    </p>
                </div>
            </div>


            <div class="bg-white mb-10 mx-auto max-w-sm rounded-xl overflow-hidden shadow-lg">
                <div class="px-6 py-4">
                    <div class="font-bold text-xl mb-2">2-step verification passkeys</div>
                    <p class="text-gray-700 text-base">
                    Qr Code is used during the configuration of two-step authentication security by various websites and applications
                    </p>
                </div>
            </div>


            <div class="bg-white mb-10 mx-auto max-w-sm rounded-xl overflow-hidden shadow-lg">
                <div class="px-6 py-4">
                    <div class="font-bold text-xl mb-2">Online accounts authentication</div>
                    <p class="text-gray-700 text-base">
                    websites can display a QR code which a registered user can scan with his or her smartphone and automatically log in
                    </p>
                </div>
            </div>

         </div>
    </div>
    <Footer />
</template>

<script>
import Footer from "../components/Footer.vue";

export default {
  name: "Usage",
  components: {
      Footer
  }
};
</script>