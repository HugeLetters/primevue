<template>
    <DocComponent title="Vue ProgressBar Component" header="ProgressBar" description="ProgressBar is a process status indicator." :componentDocs="docs" :apiDocs="['ProgressBar']" :ptTabComponent="ptComponent" :themingDocs="themingDoc" />
</template>

<script>
import ThemingDoc from '@/doc/Progressbar/theming/index.vue';
import AccessibilityDoc from '@/doc/progressbar/AccessibilityDoc';
import BasicDoc from '@/doc/progressbar/BasicDoc';
import DynamicDoc from '@/doc/progressbar/DynamicDoc';
import ImportDoc from '@/doc/progressbar/ImportDoc';
import IndeterminateDoc from '@/doc/progressbar/IndeterminateDoc';
import TemplateDoc from '@/doc/progressbar/TemplateDoc';
import PTComponent from '@/doc/progressbar/pt/index.vue';

export default {
    data() {
        return {
            docs: [
                {
                    id: 'import',
                    label: 'Import',
                    component: ImportDoc
                },
                {
                    id: 'basic',
                    label: 'Basic',
                    component: BasicDoc
                },
                {
                    id: 'dynamic',
                    label: 'Dynamic',
                    component: DynamicDoc
                },
                {
                    id: 'template',
                    label: 'Template',
                    component: TemplateDoc
                },
                {
                    id: 'indeterminate',
                    label: 'Indeterminate',
                    component: IndeterminateDoc
                },
                {
                    id: 'accessibility',
                    label: 'Accessibility',
                    component: AccessibilityDoc
                }
            ],
            ptComponent: PTComponent,
            themingDoc: ThemingDoc
        };
    }
};
</script>
