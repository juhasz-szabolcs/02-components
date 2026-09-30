<script setup>
    import { ref, reactive } from 'vue';

    import MainNavigation from './components/MainNavigation.vue';
    import SiteFooter from './components/SiteFooter.vue';
    import SiteContent from './components/SiteContent.vue';
    import InputField from './components/InputField.vue';

    // function logMessage(name) {
    //     // console.log('Input field changed!', name);
    //     console.log(name);
    // }

    function submitForm() {
        console.log('Form submitted!', formData);
        console.log('Form submitted!', JSON.stringify(formData));
    }

    const formData = reactive({
        email: '',
        firstname: '',
        lastname: ''
    });
</script>

<template>
    <header>
        <MainNavigation/>
    </header>

    <main>
        <SiteContent />
        <!-- email input -->
        <InputField 
            v-model="formData.email"
            id="e-mail"
            type="email"
            placeholder="Enter your email"
            label="Email adress"
        />

        <!-- firstname input -->
        <InputField 
            v-model="formData.firstname"
            id="firstname"
            type="text"
            placeholder="Enter your first name"
            label="First name"
        />

        <!-- lastname input -->
        <InputField 
            v-model="formData.lastname"
            id="lastname"
            type="text"
            placeholder="Enter your last name"
            label="Last name"
        />

        <button @click="submitForm">Submit</button>
    </main>


    <footer>
        <!-- sitefooter komponens használata -->
        <SiteFooter />
    </footer>

</template>

<style scoped>
</style>
