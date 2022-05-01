<script setup>
defineProps({
    title: {
        type: String
    },
    description: {
        type: String
    },
    url: {
        type: String
    },
    isPrivate: {
        type: Boolean
    }
})
</script>

<template>
    <div class="card w-96 bg-base-100 shadow-xl">
        <div class="card-body">
            <h2 class="card-title">{{ title }}</h2>
            <p> {{ description != "" ? description : 'No description' }}</p>
            <div class="card-actions justify-end">
                <a :href=link class="btn btn-primary" :disabled="isPrivate">
                    {{ isPrivate ? 'Private Repository' :
                            'View Repository'
                    }}
                </a>
            </div>
        </div>
    </div>
</template>