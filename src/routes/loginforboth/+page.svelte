<script>
    import { goto } from '$app/navigation';
</script>

<main class="flex flex-col items-center justify-center min-h-screen bg-gradient-to-b from-blue-900 via-indigo-800 to-purple-900 text-white py-12 px-6">
    <h1 class="text-4xl font-extrabold text-center mb-10 tracking-wide">Login Portal</h1>
    
    <div class="grid grid-cols-1 md:grid-cols-2 gap-12 w-full max-w-6xl">
        <!-- CIT Students -->
        <div class="flex flex-col items-center p-8 bg-blue-700 rounded-xl shadow-lg text-center w-96 transform transition duration-300 hover:scale-105">
            <h2 class="text-2xl font-semibold mb-4"> CIT Students</h2>
            <p class="text-base text-gray-200">Join workshops, courses, and collaborative learning opportunities.</p>
            <button on:click={() => goto('/loginforstudents')} 
                class="mt-6 py-3 px-6 bg-white text-blue-800 font-semibold rounded-lg w-full transition duration-300 hover:bg-gray-200">
                Login
            </button>
        </div>
        
        <!-- Non-CIT Students -->
        <div class="flex flex-col items-center p-8 bg-green-700 rounded-xl shadow-lg text-center w-96 transform transition duration-300 hover:scale-105 md:ml-auto">
            <h2 class="text-2xl font-semibold mb-4"> Non-CIT Students</h2>
            <p class="text-base text-gray-200">Access exclusive CIT resources, Problem Statements, and Progress.</p>
            <button on:click={() => goto('/loginforstudents')} 
                class="mt-6 py-3 px-6 bg-white text-green-800 font-semibold rounded-lg w-full transition duration-300 hover:bg-gray-200">
                Login
            </button>
        </div>
    </div>
</main>
