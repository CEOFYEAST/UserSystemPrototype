<template>
    <div class="root">

        <form id="sign-in-form" class="flex column">
            <input type="email" placeholder="Email" id="user-email" name="userEmail" required><br>
            <input type="password" placeholder="Password" id="user-password" name="userPassword" required><br>
            <div id="submit-container" class="flex">
                <div class="x3"></div>
                <button id="submit" type="submit" class="x2">Submit</button>
                <div class="x3"></div>
            </div>
            <div id="create-account-pointer-container">
                <p id="create-account-pointer-link">Don't have an account? Create one.</p>
                <p id="create-account-pointer">Creating an account allows you to store production vals. for up to three factories across sessions.</p>
            </div>
        </form>

    </div>
</template>

<script>
import TopNav from '@/components/TopNav.vue'

export default {
    name: 'sign in form',
    components: {
        TopNav
    }
}
</script>


<style scoped>
    input {
        font-size: 16px;
        padding-left:5px;
    }

    #submit {
        height: 25px;
    }
</style>