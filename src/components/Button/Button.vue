<script setup>
import { props } from 'vue-property-decorator'
import { ref } from 'vue'
const primary = ref(false)
function returnButtonType() {
    return {
        if(primary) { 'primary' };
        else if(secondary) { 'secondary' };
        else if(success) { 'success' };
        else if(danger) { 'danger' };
        else if(warning) { 'warning' };
        else if(info) { 'info' };
        else if(light) { 'light' };
        else if(dark) { 'dark' };
        else if(link) { 'link' };
    }
}
</script>
<template>
    <button type="button" :class="returnButtonType">Primary</button>
</template>