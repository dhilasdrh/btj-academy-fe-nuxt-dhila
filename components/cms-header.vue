<template>
    <!-- HEADER -->
    <header class="px-5 py-3 bg-blue-500 sm:py-2 flex flex-col sm:flex-row items-center justify-between">
        <!-- Logo -->
        <div class="flex items-center space-x-2">
            <img id="logoImg" class="w-16" src="assets/img/illustration.png" alt="Logo Image">
            <h2 id="logoTitle" class="text-2xl font-bold text-white">Dashboard</h2>
        </div>
        <!-- Navbar -->
        <nav class="text-md space-x-6">
            <button class="px-3 py-1 text-lg text-white">John Doe</button>
            <button @click="doLogout" class="px-6 py-2 text-md rounded-md bg-blue-700 hover:bg-blue-900 text-white ">Logout</button>
        </nav>
    </header>
</template>

<script>
export default {
    methods: {
        doLogout() {
            navigateTo('/').catch(err => {
                console.error('Error navigating to /:', err)
            });
            alert('Logging Out and Redirecting to Home Page')
        }
    }
}
</script>