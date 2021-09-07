<template>
    <v-app>
        <v-parallax src="../Assets/mac.jpg" height="700">
            <ProfileCard />
        </v-parallax>

        <SectionTitle title="Timeline" />
        <Timeline />

        <v-btn fab class=".text-secondary" v-on:click="changeTheme" fixed right bottom>
            <svg
                xmlns="http://www.w3.org/2000/svg"
                width="25"
                height="25"
                fill="currentColor"
                class="bi bi-paint-bucket"
                viewBox="0 0 16 16"
            >
                <path
                    d="M6.192 2.78c-.458-.677-.927-1.248-1.35-1.643a2.972 2.972 0 0 0-.71-.515c-.217-.104-.56-.205-.882-.02-.367.213-.427.63-.43.896-.003.304.064.664.173 1.044.196.687.556 1.528 1.035 2.402L.752 8.22c-.277.277-.269.656-.218.918.055.283.187.593.36.903.348.627.92 1.361 1.626 2.068.707.707 1.441 1.278 2.068 1.626.31.173.62.305.903.36.262.05.64.059.918-.218l5.615-5.615c.118.257.092.512.05.939-.03.292-.068.665-.073 1.176v.123h.003a1 1 0 0 0 1.993 0H14v-.057a1.01 1.01 0 0 0-.004-.117c-.055-1.25-.7-2.738-1.86-3.494a4.322 4.322 0 0 0-.211-.434c-.349-.626-.92-1.36-1.627-2.067-.707-.707-1.441-1.279-2.068-1.627-.31-.172-.62-.304-.903-.36-.262-.05-.64-.058-.918.219l-.217.216zM4.16 1.867c.381.356.844.922 1.311 1.632l-.704.705c-.382-.727-.66-1.402-.813-1.938a3.283 3.283 0 0 1-.131-.673c.091.061.204.15.337.274zm.394 3.965c.54.852 1.107 1.567 1.607 2.033a.5.5 0 1 0 .682-.732c-.453-.422-1.017-1.136-1.564-2.027l1.088-1.088c.054.12.115.243.183.365.349.627.92 1.361 1.627 2.068.706.707 1.44 1.278 2.068 1.626.122.068.244.13.365.183l-4.861 4.862a.571.571 0 0 1-.068-.01c-.137-.027-.342-.104-.608-.252-.524-.292-1.186-.8-1.846-1.46-.66-.66-1.168-1.32-1.46-1.846-.147-.265-.225-.47-.251-.607a.573.573 0 0 1-.01-.068l3.048-3.047zm2.87-1.935a2.44 2.44 0 0 1-.241-.561c.135.033.324.11.562.241.524.292 1.186.8 1.846 1.46.45.45.83.901 1.118 1.31a3.497 3.497 0 0 0-1.066.091 11.27 11.27 0 0 1-.76-.694c-.66-.66-1.167-1.322-1.458-1.847z"
                />
            </svg>
        </v-btn>
        <!-- <v-container>

        </v-container>
        <v-container>
            <v-row justify="center">
                <v-expansion-panels popout>
                    <v-expansion-panel v-for="(item, i) in 5" :key="i">
                        <v-expansion-panel-header>Item</v-expansion-panel-header>
                        <v-expansion-panel-content>
                            Content
                        </v-expansion-panel-content>
                    </v-expansion-panel>
                </v-expansion-panels>
            </v-row>
        </v-container>
        <v-container>
            <v-v-containerider></v-v-containerider>
            <v-subheader>Tech Stack</v-subheader>
            <v-divider></v-divider>

            <v-chip-group>
                <v-chip class="ma-3" color="orange" text-color="white">
                    <v-icon left>
                        mdi-label
                    </v-icon>
                    SwiftUI
                </v-chip>
                <v-chip class="ma-3" color="orange" text-color="white">
                    <v-icon left>
                        mdi-label
                    </v-icon>
                    SwiftUI
                </v-chip>
                <v-chip class="ma-3" color="orange" text-color="white">
                    <v-icon left>
                        mdi-label
                    </v-icon>
                    SwiftUI
                </v-chip>
            </v-chip-group>
        </v-container> -->
    </v-app>
</template>

<script>
import Timeline from "@/components/Timeline";
import SectionTitle from "@/components/SectionTitle";
import ProfileCard from "@/components/ProfileCard";
import Veutify from "./plugins/vuetify";
export default {
    name: "App",

    components: { Timeline, SectionTitle, ProfileCard },

    data: () => ({}),
    methods: {
        changeTheme: () => {
            console.log("On click");
            console.log(Veutify);
            Veutify.framework.theme.isDark = !Veutify.framework.theme.isDark;
        },
    },
};
</script>

// years: [ // { // type: "star", // color: "cyan", // tag: "2018-01-14", // entity: "(Computer Science - Cairo
University)", // content: // "It was the start of my lifelong learning journey that sparked my love for programming. I
graduated in 2019 with a grade of Very Good.", // }, // { // type: "star", // color: "green", // tag: "2018-01-14", //
entity: "(iOS Developer - KickstartInteractive)", // content: // "My first professional job in the summer of 2017. While
there I worked on VKader as an iOS developer. A great learning experience and a challenging project in terms of scale
and size. I gained a lot of experience over the course of completing the App.", // }, // { // type: "star", // color:
"pink", // tag: "2018-01-14", // entity: "(iOS Developer - IntCore)", // content: // "Next summer I was part of the
IntCore iOS team working on SnapCars which was a different experience. It was a collaborative experience that taught me
how to pay attention to the details no matter how small.", // }, // { // type: "star", // color: "amber", // tag:
"2018-01-14", // entity: "(Computer Science - Cairo University)", // content: // "The year I graduated from college. I
was working on my graduation project with 4 other teammates. The idea was to predict whether the skin shown in the photo
was benign or malignant of skin cancer. We trained a model on a dataset containing 55+GB of Images.", // }, // { //
type: "star", // color: "orange", // tag: "2018-01-14", // entity: "", // content: // " (Research Center - Egyptian
Armed Forces) From June 2020 until June 2021 I was doing my mandatory military service. I was lucky enough to be in a
place where programming was a viable option. I was mostly working with web technologies such as HTML, CSS, Javascript
and both SQL and NoSQL databases. I worked on different kinds of classified projects it helped develop my software
engineering skills and taught me a lot about handling complexity. It was a tough environment with lots of tasks and
pressure to get things out quickly and correctly. I learned constant iterations are the best way to improve a software
project and also a lot of team working skills and other soft skills as well as technical.", // }, // ],
