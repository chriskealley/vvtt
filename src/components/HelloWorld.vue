<script setup lang="ts">
import { ref } from 'vue'

defineProps<{ msg: string }>()

const count = ref(0)
</script>

<template>
    <h1>{{ msg }}</h1>

    <p>
        Recommended IDE setup:
        <a
            class="text-green-500"
            href="https://code.visualstudio.com/"
            target="_blank"
            >VSCode</a
        >
        +
        <a
            class="text-green-500"
            href="https://github.com/johnsoncodehk/volar"
            target="_blank"
            >Volar</a
        >
        +
        <a
            class="text-green-500"
            href="https://github.com/tailwindlabs/tailwindcss-intellisense"
            target="_blank"
            >Tailwind</a
        >
    </p>

    <p>
        See <code class="py-1 px-2 rounded-sm bg-gray-100">README.md</code> for
        more information.
    </p>

    <p>
        <a
            class="text-green-500"
            href="https://vitejs.dev/guide/features.html"
            target="_blank"
        >
            Vite Docs
        </a>
        |
        <a class="text-green-500" href="https://v3.vuejs.org/" target="_blank"
            >Vue 3 Docs</a
        >
        |
        <a
            class="text-green-500"
            href="https://tailwindcss.com/"
            target="_blank"
            >Tailwind Docs</a
        >
    </p>

    <button
        class="
            bg-green-500
            text-white
            px-4
            py-2
            my-2
            rounded-sm
            shadow-lg
            hover:bg-green-600
        "
        type="button"
        @click="count++"
    >
        count is: {{ count }}
    </button>
</template>
