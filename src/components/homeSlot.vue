<template>
    <!-- <h1>Home Slot vue js 3</h1>

    <ChildSlot>
        <h1>hello slot</h1>
    </ChildSlot>
    <ChildSlot>
        <img src="" alt="" style="height: 200px;">
    </ChildSlot>
    <ChildSlot>
        <a href="#" target="_blank" rel="noopener noreferrer">data with slot </a>
    </ChildSlot> -->
    <ChildSlot>
        <template v-slot:header>
            <h1>Amaar ul haq</h1>
        </template>
    </ChildSlot>

</template>



<script>
import ChildSlot from './ChildSlot.vue';
export default {
    name: 'homeSlot',
    components: {
        ChildSlot
    }
}
</script>