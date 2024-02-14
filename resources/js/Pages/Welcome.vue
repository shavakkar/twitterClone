<script setup>
import { Head, Link } from "@inertiajs/vue3";

import TwitterLayout from "@/Layouts/TwitterLayout.vue";

import Tweet from "@/Components/Tweet.vue";
</script>

<template>
    <Head title="Welcome" />

    <TwitterLayout>
        <div class="text-white">
            <div class="flex">
                <Tweet
                    :tweet="{
                        name: 'Test',
                        handle: '@test',
                        image: 'https://randomuser.me/api/portraits/men/40.jpg',
                        tweet: 'kjhfjdhf;jhk;jdfhdjjldsgljgjfbjdbfvkdvfjshfkhgljghflehgfjehgfjh',
                        file: '/video/warrior.mp4',
                        is_video: true,
                        comments: '35',
                        retweets: '34',
                        likes: '88',
                        analytics: '81',
                    }"
                />
            </div>
            <div class="border-b border-b-gray-800 mt-2"></div>
        </div>
    </TwitterLayout>
</template>
