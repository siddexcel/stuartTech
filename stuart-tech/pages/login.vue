<template>
    <div class="w-full px-5 pb-9 min-h-screen flex flex-col  items-center">

        <img src="../assets/images/logo.png" alt="Logo" class="size-40 mt-12" />
        <h1 class="text-2xl text-slate-200 mt-16 mb-6  ">Login</h1>
        <Input class="w-full mt- mb-4" placeholder="Email" v-model="email" />
        <Input class="w-full mb-4" placeholder="password" type="password" v-model="password" />
        <Button class="mt-auto">
            Log In
        </Button>
        <nuxt-link class="text-sm text-slate-200 mt-4">Forget your password?</nuxt-link>
        <nuxt-link class="text-sm text-slate-200 mt-3" to="/signUp" >Sign Up</nuxt-link>
    </div>
</template>

<script setup>
import { ref } from 'vue';
import Button from '../components/button.vue'
import Input from '../components/input.vue'

const email = ref('')
const password = ref('')
</script>