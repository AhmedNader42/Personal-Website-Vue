<template>
    <div>
        <v-card class="mx-auto" max-width="344">
            <v-img src="../../Assets/me.jpg" height="300px"></v-img>

            <v-card-title>
                Ahmed Nader
            </v-card-title>

            <v-card-subtitle>
                iOS Developer
            </v-card-subtitle>

            <v-card-actions>
                <v-btn :href="`mailto:ahmednader111@gmail.com`" color="orange lighten-2" text>
                    Contact
                </v-btn>

                <v-spacer></v-spacer>

                <v-btn icon @click="show = !show">
                    <v-icon>{{ show ? "mdi-chevron-up" : "mdi-chevron-down" }}</v-icon>
                </v-btn>
            </v-card-actions>

            <v-expand-transition>
                <div v-show="show">
                    <v-divider></v-divider>

                    <v-card-text>
                        <p class="text-secondary fs-6 center">
                            Software Engineer with industry experience developing large-scale complex apps and
                            contributing to open source. A team player; skilled at taking projects to the next level by
                            constantly iterating and improving them; Offering fresh ideas and out of the box thinking.
                            Communication is a must in making great products.
                        </p>
                    </v-card-text>
                </div>
            </v-expand-transition>
        </v-card>
    </div>
</template>

<script>
export default {
    name: "ProfileCard",
    data: () => ({
        show: false,
    }),
};
</script>
