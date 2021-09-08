<template>
    <v-row style="padding: 10px; margin 10px">
        <v-expansion-panels inset>
            <v-expansion-panel v-for="item in items" :key="item.title">
                <v-expansion-panel-header>
                    <p class="fs-3">
                        {{ item.title }}
                    </p></v-expansion-panel-header
                >

                <v-expansion-panel-content>
                    <v-slide-group style="margin: 10px;">
                        <v-slide-item v-for="tech in item.tech_stack" :key="tech">
                            <v-btn class="mx-2 fs-5" :input-value="active" color="primary">
                                {{ tech }}
                            </v-btn>
                        </v-slide-item>
                    </v-slide-group>

                    <v-img
                        contain
                        v-if="item.preview != undefined"
                        :src="require(`../assets/${item.preview}`)"
                        max-height="700px"
                    ></v-img>
                    <v-btn
                        v-if="item.link != undefined"
                        :href="item.link"
                        x-large
                        elevation="5"
                        color="secondary"
                        style="margin: 10px; padding: 10px"
                    >
                        Demo
                    </v-btn>
                    <v-btn
                        v-if="item.code != undefined"
                        :href="item.code"
                        x-large
                        elevation="5"
                        color="secondary"
                        style="margin: 10px; padding: 10px"
                    >
                        Code
                    </v-btn>
                </v-expansion-panel-content>
            </v-expansion-panel>
        </v-expansion-panels>
    </v-row>
</template>

<script>
export default {
    name: 'ProjectPreview',
    data: () => ({
        items: [
            {
                title: 'Bank (Full-Stack Website)',
                preview: 'Bank.png',
                tech_stack: ['Python', 'Vue', 'Django', 'DjangoRestFramework', 'Vuetify', 'Stripe'],
                link: 'https://www.youtube.com/watch?v=hQmGF3IvkT0',
                code: 'https://github.com/AhmedNader42/bank',
            },
            {
                title: 'Hacker New Clone (Server-side rendered website)',
                preview: 'hacker_news_clone.png',
                tech_stack: ['Javascript', 'NextJS', 'Express', 'Axios', 'NodeJS'],
                code: 'https://github.com/AhmedNader42/hacker-news-clone',
            },
            {
                title: 'SnapCars (iOS App)',
                preview: 'SnapCars.png',
                tech_stack: [
                    'Swift',
                    'MVVM',
                    'Storyboards',
                    'CoreData',
                    'CoreAnimation',
                    'AlamoFire',
                    'Kingfisher',
                    'GoogleMaps SDK',
                ],
                link: 'https://intcore.com/Snapcars-Mobile-App/',
            },
            {
                title: 'VKader (iOS App)',
                tech_stack: [
                    'Swift',
                    'MVC',
                    'Storyboards',
                    'AlamoFire',
                    'Kingfisher',
                    'GoogleMaps SDK',
                ],
                link:
                    'https://appadvice.com/game/app/vkader-d9-81-d9-8a-d9-83-d8-a7-d8-af-d8-b1/1300676456',
                preview: 'Vkader.png',
            },
            {
                title: 'Tinder Clone (iOS App)',
                tech_stack: ['Swift', 'SwiftUI', 'Kingfisher'],
                preview: 'Tinder.png',
                link:
                    'https://drive.google.com/file/d/1qpvWe0uas18DeM9-xyjGsQrMiBjA7QZh/view?usp=sharing',
                code: 'https://github.com/AhmedNader42/TinderClone',
            },
            {
                title: 'Breakpoint (iOS App)',
                preview: 'Breakpoint.png',
                tech_stack: ['Swift', 'UIKit', 'Programmatic UI', 'Firebase', 'Google Sign-In'],
                link:
                    'https://drive.google.com/file/d/1tZCcsSc6l0e2409Gp64Gn0elTiNKx48S/view?usp=sharing',
                code: 'https://github.com/AhmedNader42/_BreakPoint',
            },
            {
                title: 'Rocket.Chat.Watch (WatchOS App)',
                tech_stack: ['WatchKit', 'AlamoFire', 'UserNotifications', 'Swift'],
                link:
                    'https://drive.google.com/file/d/1tOY_RcaAN9T3NDcq9dpFkjxAVcGHBW-v/view?usp=sharing',
                code: 'https://github.com/AhmedNader42/Rocket.Chat.Watch',
            },
            {
                title: 'Swift Algorithms club (Algorithm)',
                preview: 'SAC.png',
                tech_stack: ['Swift'],
                code:
                    'https://github.com/raywenderlich/swift-algorithm-club/tree/master/Closest%20Pair',
            },
        ],
    }),
};
</script>
