<template>
    <DocSectionText v-bind="$attrs">
        <p>Theming is implemented with the pass through properties in unstyled mode. Example below demonstrates the built-in Tailwind theme.</p>
    </DocSectionText>
    <DocSectionCode :code="code" embedded />
</template>

<script>
export default {
    data() {
        return {
            date: null,
            code: {
                composition: `
<template>
    <div class="card flex justify-center">
        <Calendar v-model="date" />
    </div>
</template>

<script setup>
import { ref } from "vue";

const date = ref();
<\/script>`
            }
        };
    }
};
</script>
