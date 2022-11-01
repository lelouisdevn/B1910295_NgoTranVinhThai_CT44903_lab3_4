<script>
export default {
    props: {
        contact: {type: Object, required: true },
    },
};
</script>

<template>
    <div>
        <div class="p-1">
            <strong>Ten:</strong>
            {{ contact.name }}
        </div>
        <div class="p-1">
            <strong>Email:</strong>
            {{ contact.email }}
        </div>
        <div class="p-1">
            <strong>Dia chi:</strong>
            {{ contact.address }}
        </div>
        <div class="p-1">
            <strong>Dien thoai:</strong>
            {{ contact.phone }}
        </div>
        <div class="p-1">
            <strong>Lien he yeu thich:&nbsp;</strong>
            <i v-if="contact.favorite" class="fas fa-check"></i>
            <i class="fas fa-times" v-else></i>
        </div>
    </div>
</template>