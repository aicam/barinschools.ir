<template>
    <v-container>
        <v-card>
            <v-app-bar
                    color="#0082FF"
            >
                <v-card-title style="color: aliceblue;">آشنایی با بنیاد برین</v-card-title>
            </v-app-bar>
            <v-card-text>
                <v-row>
                    <v-col>
                        <p class="info_barin">
                    بنیاد نیکوکاری برین شمیرانات (صالح)  یکی از مؤسسات خیریه‌ای است که با هدف اصلی مدرسه‌سازی، در سال ۱۳۹۰ زیر نظر سازمان بهزیستی تهران فعالیت خود را در راستای حمایت از آموزش و تحصیل کودکان و نوجوانان بدسرپرست و بی‌سرپرست آغاز کرد.  در این برهه کوتاه نزدیک به ده ساله، بنیاد برین در امور خیر بسیار زیادی به طور مستقیم و غیرمستقیم نقش داشته است. این بنیاد در طی 8 سال گذشته، بیش از 1000 دانش‌آموز از مقطع ابتدایی تا دانشگاه را تحت پوشش خود قرار داده است و در ساخت و بهره‌برداری از 20 مدرسه، به صورت مستقیم، نقش داشته است.
                        </p>
                    </v-col>
                    <v-col>
                    <v-img
                        :src="barin_info"></v-img>
                    </v-col>
                </v-row>
            </v-card-text>
        </v-card>
    </v-container>
</template>

<script>
    export default {
        name: "BarinInfo",
        data: () => ({
            barin_info: require('../assets/barin_info.jpg')
        })
    }
</script>

<style scoped>
    .info_barin {
        font-size: 18px;
        color: #0b0422;
    }
</style>
