<template>
    <div class="grid grid-cols-2">
        <div class="font-bold text-xl">
            {{ selected.name }} Chat
        </div>
    </div>

</template>
<script>
export default {
    props: ['rooms', 'currentRoom'],
    data: function() {
        return {
            selected: ''
        }
    },
    created() {
        this.selected = this.currentRoom;
    }
}
</script>