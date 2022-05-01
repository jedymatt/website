<script setup>
import { RouterLink, RouterView } from 'vue-router'
import { ExternalLinkIcon } from '@heroicons/vue/outline'
</script>

<template>
  <div class="min-h-screen">
    <header>
      <div class="navbar bg-base-100">
        <div class="flex-1">
          <RouterLink to="/" class="btn btn-ghost normal-case text-xl">jedymatt</RouterLink>
        </div>
        <div class="flex-none">
          <ul class="menu menu-horizontal p-0">
            <li>
              <RouterLink to="/about-me">About Me</RouterLink>
            </li>
            <li>
              <RouterLink to="/projects">Projects</RouterLink>
            </li>
            <li>
              <a href="http://www.github.com/jedymatt" target="_blank" rel="noopener noreferrer">
                Github
                <ExternalLinkIcon class="h-5 w-5" />
              </a>
            </li>
          </ul>
        </div>
      </div>
    </header>

    <RouterView />
  </div>
</template>