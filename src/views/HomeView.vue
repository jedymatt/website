<script setup>
import { RouterLink } from 'vue-router';
import { UserIcon, CollectionIcon } from '@heroicons/vue/outline';
</script>

<template>
    <div class="my-4">
        <div>
            <div class="flex justify-center">
                <span class="text-6xl font-bold text-center">Hi, I'm Jedy Matt Tabasco</span>
            </div>
            <div class="mt-4">
                <p class="text-center text-xl">
                    A passionate programmer who tries different technologies.
                </p>
            </div>
        </div>
        <div class="mt-4 flex justify-center ">
            <div class="grid grid-rows-">
                <RouterLink to="/about-me" class="btn btn-primary">
                    About Me
                    <UserIcon class="ml-2 h-5 w-5" />
                </RouterLink>
                <div class="mt-4">
                    <RouterLink to="/projects" class="btn btn-primary">
                        Projects
                        <CollectionIcon class="ml-2 h-5 w-5" />
                    </RouterLink>
                </div>
            </div>
        </div>
    </div>


</template>
