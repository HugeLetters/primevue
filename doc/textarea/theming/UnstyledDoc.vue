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
            value: '',
            code: {
                composition: `
<template>
    <div class="card flex justify-center">
        <Textarea v-model="value" rows="5" cols="30" />
    </div>
</template>

<script setup>
import { ref } from 'vue';

const value = ref('');
<\/script>`
            }
        };
    }
};
</script>
