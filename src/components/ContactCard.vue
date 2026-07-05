<script>
    export default {
        props: {
           contact: {
                type: Object,
                required: true
            }, 
        },
    };
</script>

<template>
    <div>   
        <div class="p-1">
            <strong>Tên: {{ contact.name }}</strong> 
        </div>
        <div class="p-1">
            <strong>Email: {{ contact.email }}</strong> 
        </div>
        <div class="p-1">
            <strong>Địa chỉ: {{ contact.address }}</strong> 
        </div>
        <div class="p-1">
            <strong>Điện thoại: {{ contact.phone }}</strong> 
        </div>
        <div class="p-1">
            <strong>Liên hệ yêu thích: &nbsp </strong>
            <i v-if="contact.isFavorite" class="fas fa-check"></i>
            <i v-else class="fas fa-times"></i>
        </div>
    </div>
</template>