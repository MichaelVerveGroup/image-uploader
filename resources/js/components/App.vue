<template>
    <div class="mt-4">
        <file-pond name="image" ref="pond" label-idle="Click to chose image, or drag here..." server="/upload"
            @init="filepondInitalised" />
    </div>
</template>
<script>
import vueFilePond from 'vue-filepond';
import "filepond/dist/filepond.min.css";
import FilePondPluginFileValidateType from 'filepond-plugin-file-validate-type';

const FilePond = vueFilePond(FilePondPluginFileValidateType);

export default {
    components: {
        FilePond
    },
    data() {
        return {

        }
    },
    methods: {
        filepondInitialised() {

        }
    }
}
</script>