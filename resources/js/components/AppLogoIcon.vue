<script setup lang="ts">
import type { HTMLAttributes } from 'vue';

defineOptions({
    inheritAttrs: false,
});

interface Props {
    className?: HTMLAttributes['class'];
}

defineProps<Props>();
</script>

<template>
    <img
        src="/storage/images/logo.png"
        :class="className"
        v-bind="$attrs"
        alt="Logo de la aplicación"
    />
</template>
