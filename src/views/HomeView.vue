<script setup>
import {  ref, reactive} from "vue";
import NavigationMain from "@/components/NavigationMain.vue";

const name = ref('Luiz Balisa')
const age = ref('22')

const person = reactive({
    name,
    age,
});

</script>

<template>
    <div>
        <navigation-main />
        <p class=" ">{{ person.name }}</p>
        <p>{{ person.age }}</p>
    </div>
</template>

<style lang="scss" scoped>
 p {
	 color: var(--color-primary);
	 font-size: 2rem;
 }
</style>