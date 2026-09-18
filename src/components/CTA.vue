<script>
import { ref } from 'vue';

export default {
    props: {
        image: {
            type: Boolean,
            required: true
        }
    },
    setup() {
        const result = ref(null);
        const showResult = ref(true);
        const resultColor = ref('black');

        const handleSubmit = async (e) => {
            e.preventDefault();
            const form = e.target;
            const formData = new FormData(form);

            const object = {};
            formData.forEach((value, key) => {
                object[key] = value;
            });

            result.value = "Please wait...";
            resultColor.value = 'black';
            showResult.value = true;

            try {
                const response = await fetch("https://api.web3forms.com/submit", {
                    method: "POST",
                    headers: {
                        "Content-Type": "application/json",
                        Accept: "application/json"
                    },
                    body: JSON.stringify(object)
                });

                const json = await response.json();

                if (response.status == 200) {
                    result.value = json.message;
                    resultColor.value = 'green';
                } else {
                    console.log(response);
                    result.value = json.message;
                    resultColor.value = 'red';
                }

                form.reset();
                setTimeout(() => {
                    showResult.value = false;
                }, 5000);

            } catch (error) {
                console.log(error);
                result.value = "Something went wrong!";
                resultColor.value = 'red';
            }
        };

        return {
            result,
            showResult,
            resultColor,
            handleSubmit
        };
    }
}
</script>


<template>
    <div class="bgimagepic m-4">
        <div class="bg-black/20 m-10 rounded-2xl border border-white/20 max-w-5xl mx-auto">
            <section class="text-white p-10">
                <h2 class="uppercase md:text-4xl text-2xl text-center font-light">
                    Email me for dyslexia services in newton abbot and devon.
                </h2>

                <p class="text-center mt-4 italic font-light opacity-80">
                    Fill in the contact form below to receive a free quote. I am
                    always more than happy to help.
                </p>
            </section>

            <form @submit="handleSubmit" action="https://api.web3forms.com/submit" method="POST" id="form"
                class="max-w-3xl mx-auto px-6 flex flex-col gap-4">
                <div class="flex flex-col md:flex-row gap-4">
                    <input name="name" type="text" placeholder="Name" required
                        class="flex-1 p-5 rounded-2xl bg-white/5 text-white placeholder-white/50 border-2 border-white/10 outline-none focus:border-white/30 focus:bg-white/10 transition-all duration-300 backdrop-blur-md">

                    <input name="email" type="email" placeholder="Email" required
                        class="flex-1 p-5 rounded-2xl bg-white/5 text-white placeholder-white/50 border-2 border-white/10 outline-none focus:border-white/30 focus:bg-white/10 transition-all duration-300 backdrop-blur-md">

                    <input name="number" type="number" placeholder="Phone Number" required
                        class="flex-1 p-5 rounded-2xl bg-white/5 text-white placeholder-white/50 border-2 border-white/10 outline-none focus:border-white/30 focus:bg-white/10 transition-all duration-300 backdrop-blur-md">
                </div>

                <input type="text" name="honeypot" style="display:none">
                <input type="checkbox" name="botcheck" class="hidden" style="display: none;">
                <input type="hidden" name="access_key" value="5dff5abc-bfb3-4e4c-b6b1-6fd72ba7d2a2">

                <!-- <input type="hidden" name="redirectTo" value="https://www.rhdyslexiaservices.co.uk/contact-success"> -->

                <textarea name="message" placeholder="Message"
                    class="w-full p-5 rounded-2xl bg-white/5 text-white backdrop-blur-md placeholder-white/50 border-2 border-white/10 outline-none focus:border-white/30 focus:bg-white/10 transition-all duration-300 min-h-[180px] resize-y"></textarea>

                <button type="submit" value="Send message"
                    class="backdrop-blur-md bg-blue-500/40 border border-white/20 cursor-pointer px-14 py-2 rounded-full my-4 mb-7 font-light transition-all duration-300 text-white w-fit mx-auto text-lg shadow-xl transform hover:-translate-y-1 active:translate-y-0">
                    Send Message
                </button>

                <div v-if="showResult" :style="{ color: resultColor }" class="text-center mt-4 !text-white font-bold">
                    {{ result }}
                </div>
            </form>
        </div>
    </div>
</template>

<style>
.bgimagepic {
    position: relative;
    overflow: hidden;
}

.bgimagepic::before {
    content: "";
    position: absolute;
    inset: -10px;
    background-image: url('../../src/assets/flowers.png');
    background-size: cover;
    background-position: center;
    filter: blur(10px);
    opacity: 0.4;
    z-index: 0;
}

.bgimagepic>* {
    position: relative;
    z-index: 1;
}
</style>