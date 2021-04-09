<template>
    <v-container>
        <v-card>
            <v-card-text>
                <v-autocomplete
                        v-model="model"
                        :items="schools_name"
                        color="white"
                        hide-no-data
                        hide-selected
                        item-text="Description"
                        item-value="API"
                        label="نام مدرسه خود را وارد نمایید"
                        placeholder="نمونه: المهدی"
                        prepend-icon="mdi-database-search"
                        return-object
                ></v-autocomplete>
              <v-btn
                      @click="goto_school"
              >
                ورود
              </v-btn>
            </v-card-text>
        </v-card>
    </v-container>
</template>

<script>
    export default {
        name: 'search',

        data: () => ({
            model: "",
            schools_name: [
                'کوهرنگ'
            ],
        }),
        methods: {
            goto_school: function () {
                var sub = "";
                if (this.model === this.schools_name[0])
                    sub = "koohrang";
                    location.replace("https://" + sub + ".barineducation.ir/login/index.php")
            }
        }
    }
</script>
