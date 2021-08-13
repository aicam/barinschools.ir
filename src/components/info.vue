<template>
    <v-container>
        <v-card>
            <v-app-bar
                    color="#0082FF"
            >
                <v-card-title style="color: aliceblue;">سامانه آموزش آنلاین بنیاد برین</v-card-title>
            </v-app-bar>
            <v-card-text style="font-size: 18px;color: #0b0422;">
                موسسه برین در جهت ارایه آموزش به دانش آموزان محروم کشور اقدام به ایجاد یک سیستم آموزشی آنلاین کرده تا
                همه دانش آموزان
                از سراسر کشور به آموزش دسترسی داشته باشند.
                <br>
                نام مدرسه خود را مانند : "المهدی" وارد کرده و به سیستم آموزشی آنلاین هدایت خواهید شد.
                <v-container class="align-center justify-center">
                    <v-img

                            class="mx-auto"
                            :src="android_download"
                            width="200"
                    />
                </v-container>
            </v-card-text>
        </v-card>
    </v-container>
</template>

<script>
    export default {
        data: () => ({
            android_download: require('../assets/android.png')
        }),
        name: "info"
    }
</script>

<style scoped>

</style>
