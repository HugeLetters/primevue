<template>
    <DocComponent title="Vue Tag Component" header="Tag" description="Tag component is used to categorize content." :componentDocs="docs" :apiDocs="['Tag']" :ptTabComponent="ptComponent" :themingDocs="themingDoc" />
</template>

<script>
import ThemingDoc from '@/doc/Tag/theming/index.vue';
import AccessibilityDoc from '@/doc/tag/AccessibilityDoc';
import BasicDoc from '@/doc/tag/BasicDoc';
import IconDoc from '@/doc/tag/IconDoc';
import ImportDoc from '@/doc/tag/ImportDoc';
import PillDoc from '@/doc/tag/PillDoc';
import SeverityDoc from '@/doc/tag/SeverityDoc';
import TemplateDoc from '@/doc/tag/TemplateDoc';
import PTComponent from '@/doc/tag/pt/index.vue';

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
                    id: 'severity',
                    label: 'Severity',
                    component: SeverityDoc
                },
                {
                    id: 'pill',
                    label: 'Pill',
                    component: PillDoc
                },
                {
                    id: 'icons',
                    label: 'Icon',
                    component: IconDoc
                },
                {
                    id: 'template',
                    label: 'Template',
                    component: TemplateDoc
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
