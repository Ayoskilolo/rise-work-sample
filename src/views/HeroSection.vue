<script setup lang="ts">
import { Icon } from '@iconify/vue';
</script>

<template>
    <section>
        <div class="heroText">
            <div>
                <h2>
                    <span id="topline">Dollar investments</span>
                    <span id="bottomline"> that help you grow</span>
                </h2>
                <p>
                    <span id="quality">We put your money in high quality assets that help</span>
                    <span id="wealth">you build wealth and achieve your financial goals.</span>
                </p>

                <div class="buttons">
                    <div class="button">
                        <Icon icon="ic:baseline-apple" style="font-size: 45px;" />
                        <span>
                            <span class="line-break-block">Download on the </span>
                            <span class="bold">App Store</span>
                        </span>
                    </div>
                    <div class="button">
                        <Icon icon="mage:playstore" style="font-size: 40px;" />
                        <span>
                            <span class="line-break-block">Download on the</span>
                            <span class="bold line-break-block">Play Store</span>
                        </span>
                    </div>
                </div>
            </div>

            <div class="appPreview">

            </div>
            <!-- <img src="/appPreview.png" alt="" class="appPreview"> -->
        </div>

        <div id="heroPartners">
            <img src="/arm-logo.png" alt="ARM Trustees Logo" width="150px">
            <img src="/techstars-logo.png" alt="Techstars Logo" width="150px">
            <img src="/western-union-logo.png" alt="Western Union Logo" width="200px">
            <img src="/ventures-logo.png" alt="Ventures Capital Logo" width="120px">
        </div>
    </section>

</template>

<style scoped>
section {
    display: flex;
    flex-direction: column;
    height: 100svh;
}

.heroText {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex: 2;
    padding: 2rem;
}

h2 {
    font-size: 66px;
    line-height: 40px;
    color: #07969E;
    margin: 0;
}

#topline::after,
#bottomline::after {
    content: "\A";
    white-space: pre;
    display: block;
}

p {
    line-height: 15px;
    margin: 0;
    padding: 0;
    font-weight: light;
    color: #4A5050;
}

#quality::after,
#wealth::after {
    content: "\A";
    white-space: pre;
    display: block;
}

#heroPartners {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 1rem;
    filter: grayscale(90%);
}

.appPreview {
    height: 70%;
    width: 30%;
    background-image: url('/appPreview.png');
    background-position: center;
    background-size: contain;
    background-repeat: no-repeat;
}

.buttons {
    height: max-content;
    display: flex;
    gap: 1rem;
    align-items: center;
    justify-content: start;
}

.button {
    display: flex;
    height: 100%;
    border-radius: 10px;
    background-color: #2D2D2D;
    color: #FFFFFF;
    padding: 8px 8px;
}

span.button {
    margin: 0;
    padding: 0;
}

.bold {
    font-weight: bold;
}
</style>