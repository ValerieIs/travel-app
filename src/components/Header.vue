<template>
    <header class="grid grid-cols-2 items-center">
        <div class="menu_icon">
            <div></div>
            <div></div>
        </div>
        <div class="account flex items-center justify-end">
            <div class="mr-4 text-base">Hi, Stephan</div>
            <div class="avatar w-10 h-10"></div>
        </div>
    </header>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style scoped>
    .avatar {
        background: url('../assets/images/avatar.png');
        border-radius: 50%;
    }
    .menu_icon div:nth-child(1) {
        width: 27px;
    }
    .menu_icon div:nth-child(2) {
        width: 19px;
        margin-top: 6px;
    }
    .menu_icon * {
        height: 2.29px;
        background-color: black;
    }
</style>