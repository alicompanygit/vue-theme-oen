<template>
    <div class="accordion" id="accordionExample">
        <div v-for="item, id in data" class="mt-2">
            <h2 class="accordion-header rounded">
                <button type="button" data-bs-toggle="collapse" :data-bs-target="'#collapse' + id" aria-expanded="true"
                    :aria-controls="'collapse' + id"
                    class="accordion-btn w-100 d-flex justify-content-between p-3 px-3 rounded-4 align-items-center">
                    <span v-html="item.title" class="accordion-btn--text" :style="['font-size: ' + fontSize]"></span>
                    <img :src="item.iconSrc" alt="icon" class="accordion-btn--img">
                </button>
            </h2>
            <div :id="'collapse' + id" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
                <div class="accordion-body" v-html="item.description" :style="['font-size: ' + fontSize]"></div>
            </div>
        </div>
    </div>
</template>
<script setup>
import { ref, defineProps, onMounted } from 'vue';
const props = defineProps({
    data: {
        typeof: Object,
        default: [{ title: 'lorem1', description: 'lorem ipsum1 ...', iconSrc: 's' }, { title: 'lorem2', description: 'lorem ipsum2 ...', iconSrc: 's' }]
    },
    classes: {
        typeof: Array,
        default: []
    },
    fontSize: {
        typeof: String,
        default: '20px'
    }
});
onMounted(() => {
    for (let index = 0; index < props.classes.length; index++) {
        document.querySelectorAll(".accordion-btn").forEach((el) => {
            el.classList.add(props.classes[index])
        })
    }
})
</script>
<style scoped lang="scss">
.accordion-button {
    &::after {
        display: none;
    }
}

.accordion {
    &-button:not(.collapsed) {
        background-color: #ffffff00;
        border: none;
    }

    &-btn {
        border: none;
    }
}
</style>