<template>
    <div class="flex min-h-screen text-gray-700 bg-custom-bg">

        <!-- MAIN CONTAINER -->
        <div id="mainContainer" class="container m-auto w-5/6 shadow-2xl bg-white rounded-2xl overflow-auto h-[90vh]">
            <!-- HEADER -->
            <header class="px-5 py-3 sm:py-2 flex flex-col sm:flex-row items-center justify-between rounded-t-2xl">
                <!-- Logo -->
                <div class="flex items-center space-x-2">
                    <img id="logoImg" class="w-16" src="assets/img/illustration.png" alt="Logo Image">
                    <h2 id="logoTitle" class="text-2xl font-bold text-indigo-700">Welcome</h2>
                </div>
                <!-- Navbar -->
                <nav class="text-md space-x-6">
                    <button class="px-3 py-1 text-md text-blue-600 font-bold border-b-4 border-blue-500">Home</button>
                    <button @click="doLogin" class="px-6 py-2 text-md rounded-md bg-blue-700 hover:bg-blue-900 text-white ">Login</button>
                </nav>
            </header>


            <!-- MAIN CONTENT -->
            <main>
                <!-- SECTION PROFILE -->
                <section id="section-profile" class="animated-section lg:flex md:grid-cols-2 gap-5 items-center p-5">
                    <!-- Photo Profile -->
                    <div class="lg:w-5/12 items-center justify-center">
                        <img id="profileImg" class="rounded-full mx-auto max-w-[80%] grow-0" src="assets/img/profile.jpg" alt="Profile Image" >
                    </div>

                    <!-- Profile Description -->
                    <div id="profileDescription" class="flex flex-col lg:w-7/12 space-y-4 p-4 m-2 sm:p-8 text-center lg:text-left">
                        <h3 class="text-xl">Hi, my name is</h3>
                        <h1 id="name" class="text-4xl md:text-5xl font-bold text-blue-700 underline decoration-dotted decoration-yellow-400">Nur Fadhilah Sadrah.</h1>
                        
                        <p class="leading-relaxed font-normal">
                            Informatics Engineering graduate and passionate <strong>Software Developer</strong>. With a keen eye for design and a knack for coding, I bring ideas to life by building <em class="font-medium text-blue-700 italic">visually stunning and highly functional web & mobile apps</em>. I'm also interested in <abbr title="Artificial Intelligence" class="initialism">AI</abbr> and Machine Learning. In my free time, I enjoy listening to music, reading webtoons, <span class="line-through">fangirling</span>, and watching variety shows.
                        </p>

                        <div class="flex justify-center sm:justify-normal gap-3">             
                            <button id="btnGithub" class="p-3 rounded-xl border-2 bg-blue-700 hover:bg-blue-900 text-white " onclick="window.location.href='https://www.github.com/dhilasdrh'">Visit GitHub</button>
                            <button id="btnEmail" class="p-3 rounded-xl border-2 bg-blue-400 hover:bg-blue-900 text-white" onclick="window.location.href='mailto:dhilasdrh@gmail.com?subject=Greetings&body=Hello,%20Dhila!'">Send Email</button>
                        </div>
                    </div>
                </section>



                <!-- SECTION EDUCATION-->
                <section id="section-education" class="animated-section position-relative bg-blue-50 lg:flex md:grid-cols-2 gap-5 items-center p-5">
                <div class="flex flex-col lg:w-6/12 space-y-4 p-4 m-2 sm:p-8">
                    <!-- Education List Container  -->
                    <div class="relative space-y-8 before:absolute before:inset-0 before:ml-5 before:-translate-x-px before:h-full before:w-0.5 before:bg-gradient-to-b before:from-transparent before:via-slate-300 before:to-transparent">
                            <h1 class="text-4xl font-bold underline decoration-dotted decoration-yellow-400 text-blue-700">Education</h1>
                            <!-- University -->
                            <div class="relative flex items-center justify-between mb-3">
                                <div class="flex items-center justify-center w-10 h-10 rounded-full border border-white bg-blue-500 text-white shadow shrink-0">
                                    <svg class="fill-current" xmlns="http://www.w3.org/2000/svg" width="12" height="10">
                                        <path fill-rule="nonzero" d="M10.422 1.257 4.655 7.025 2.553 4.923A.916.916 0 0 0 1.257 6.22l2.75 2.75a.916.916 0 0 0 1.296 0l6.415-6.416a.916.916 0 0 0-1.296-1.296Z" />
                                    </svg>
                                </div>
                                <div class="w-full ml-5 bg-white p-4 rounded border border-slate-200 shadow">
                                    <div class="font-medium text-slate-900 mb-1">UIN Alauddin Makassar</div>
                                    <div class="text-slate-500 italic">Informatics Engineering</div>
                                </div>
                            </div>

                            <!-- Senior High School  -->
                            <div class="relative flex items-center justify-between">
                                <div class="flex items-center justify-center w-10 h-10 rounded-full border border-white bg-blue-400 text-white shadow shrink-0">
                                    <svg class="fill-current" xmlns="http://www.w3.org/2000/svg" width="12" height="10">
                                        <path fill-rule="nonzero" d="M10.422 1.257 4.655 7.025 2.553 4.923A.916.916 0 0 0 1.257 6.22l2.75 2.75a.916.916 0 0 0 1.296 0l6.415-6.416a.916.916 0 0 0-1.296-1.296Z" />
                                    </svg>
                                </div>
                                <div class="w-full ml-5 bg-white p-4 rounded border border-slate-200 shadow">
                                    <div class="font-medium text-slate-900 mb-1">SMAN 1 Sungguminasa</div>
                                    <div class="text-slate-500 italic">Math and Natural Sciences</div>
                                </div>
                            </div>

                            <!-- Junior High School -->
                            <div class="relative flex items-center justify-between">
                                <div class="flex items-center justify-center w-10 h-10 rounded-full border border-white bg-blue-500 text-white shadow shrink-0">
                                    <svg class="fill-current" xmlns="http://www.w3.org/2000/svg" width="12" height="10">
                                        <path fill-rule="nonzero" d="M10.422 1.257 4.655 7.025 2.553 4.923A.916.916 0 0 0 1.257 6.22l2.75 2.75a.916.916 0 0 0 1.296 0l6.415-6.416a.916.916 0 0 0-1.296-1.296Z" />
                                    </svg>
                                </div>
                                <div class="w-full ml-5 bg-white p-4 rounded border border-slate-200 shadow">
                                    <div class="font-medium text-slate-900 mb-1">SMPN 1 Sungguminasa</div>
                                </div>
                            </div>

                            <!-- Elementary School -->
                            <div class="relative flex items-center justify-between">
                                <div class="flex items-center justify-center w-10 h-10 rounded-full border border-white bg-blue-400 text-white shadow shrink-0">
                                    <svg class="fill-current" xmlns="http://www.w3.org/2000/svg" width="12" height="10">
                                        <path fill-rule="nonzero" d="M10.422 1.257 4.655 7.025 2.553 4.923A.916.916 0 0 0 1.257 6.22l2.75 2.75a.916.916 0 0 0 1.296 0l6.415-6.416a.916.916 0 0 0-1.296-1.296Z" />
                                    </svg>
                                </div>
                                <div class="w-full ml-5 bg-white p-4 rounded border border-slate-200 shadow">
                                    <div class="font-medium text-slate-900 mb-1">SDN Paccinongang Unggulan</div>
                                </div>
                            </div>
                            
                        </div>
                </div>

                <!-- Illustration Image -->
                    <div class="lg:w-6/12 items-center justify-center">
                        <img id="imgEducation" class="rounded-full" src="assets/img/education-1.png" alt="Graduation Illustration Image" >
                    </div>
            </section>
            

            <!-- SECTION WORK -->
                <section id="section-work" class="animated-section position-relative p-8 container mx-auto">
                    <h1 class="text-4xl font-bold underline decoration-dotted decoration-yellow-400 text-blue-700 p-3 m-5">Work Experiences</h1>
                    <div class="grid grid-cols-1 sm:grid-cols-3 gap-5 p-5">
                        <div class="mb-5">
                            <div class="icon p-3 mb-2 rounded-lg inline-block bg-blue-400 bg-opacity-50">
                                <svg xmlns="http://www.w3.org/2000/svg" height="16" width="18" viewBox="0 0 576 512"><path d="M420.6 301.9a24 24 0 1 1 24-24 24 24 0 0 1 -24 24m-265.1 0a24 24 0 1 1 24-24 24 24 0 0 1 -24 24m273.7-144.5 47.9-83a10 10 0 1 0 -17.3-10h0l-48.5 84.1a301.3 301.3 0 0 0 -246.6 0L116.2 64.5a10 10 0 1 0 -17.3 10h0l47.9 83C64.5 202.2 8.2 285.6 0 384H576c-8.2-98.5-64.5-181.8-146.9-226.6"/></svg>
                            </div>
                            <h2 class="text-xl font-bold text-blue-700">Mobile App Developer (Intern)</h2>
                            <h4 class="text-md font-medium text-slate-500 italic">Glolingo Indonesia</h4>
                            <p class="mt-3">
                                Contributed to the development of an AR Android app for language practice using <b>Kotlin</b> and <b>Firebase</b>.  Matchmaking based on user preferences like language proficiency, gender, or specific fields.
                            </p>
                        </div>

                        <div class="mb-5">
                            <div class="icon p-3 mb-2 rounded-lg inline-block bg-blue-500 bg-opacity-50">
                                <svg xmlns="http://www.w3.org/2000/svg" height="16" width="20" viewBox="0 0 640 512"><path d="M128 32C92.7 32 64 60.7 64 96V352h64V96H512V352h64V96c0-35.3-28.7-64-64-64H128zM19.2 384C8.6 384 0 392.6 0 403.2C0 445.6 34.4 480 76.8 480H563.2c42.4 0 76.8-34.4 76.8-76.8c0-10.6-8.6-19.2-19.2-19.2H19.2z"/></svg>
                            </div>
                            <h2 class="text-xl font-bold text-blue-700">Web Developer (Intern)</h2>
                            <h4 class="text-md font-medium text-slate-500 italic">IQR Foundation</h4>
                            <p class="mt-3">
                                Redesigned IQR Foundation website. Utilized <b>Figma</b> for design mockups and implemented the redesign using <b>WordPress</b> and <b>Elementor</b>, ensuring a modern and user-friendly experience.
                            </p>
                        </div>

                        <div class="mb-5">
                            <div class="icon p-3 mb-2 rounded-lg inline-block bg-blue-400 bg-opacity-50">
                                <svg xmlns="http://www.w3.org/2000/svg" height="16" width="14" viewBox="0 0 448 512"><path d="M448 80v48c0 44.2-100.3 80-224 80S0 172.2 0 128V80C0 35.8 100.3 0 224 0S448 35.8 448 80zM393.2 214.7c20.8-7.4 39.9-16.9 54.8-28.6V288c0 44.2-100.3 80-224 80S0 332.2 0 288V186.1c14.9 11.8 34 21.2 54.8 28.6C99.7 230.7 159.5 240 224 240s124.3-9.3 169.2-25.3zM0 346.1c14.9 11.8 34 21.2 54.8 28.6C99.7 390.7 159.5 400 224 400s124.3-9.3 169.2-25.3c20.8-7.4 39.9-16.9 54.8-28.6V432c0 44.2-100.3 80-224 80S0 476.2 0 432V346.1z"/></svg>
                            </div>
                            <h2 class="text-xl font-bold text-blue-700">Back End Developer (Intern)</h2>
                            <h4 class="text-md font-medium text-gray-400 italic">PT Docotel Technology Celebes</h4>
                            <p class="mt-3">
                                Worked with senior developers to implement scalable and efficient backend solutions for HR Information System using <b>Laravel</b>. Assisted in database management, utilizing <b>SQL</b> databases to organize and optimize data retrieval processes.
                            </p>
                        </div>
                    </div>
                </section>

                <!-- SECTION MOTTO -->
                <section id="section-motto" class="animated-section position-relative p-5 bg-blue-50 text-center">
                    <!-- <h1 class="text-5xl font-extrabold underline decoration-dotted decoration-yellow-400 text-blue-700">Learn. Grow. Succeed.</h1> -->
                    <figure class="max-w-screen-md mx-auto my-10">
                        <svg class="w-10 h-10 mx-auto mb-3 text-gray-400 dark:text-gray-600" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 18 14">
                            <path d="M6 0H2a2 2 0 0 0-2 2v4a2 2 0 0 0 2 2h4v1a3 3 0 0 1-3 3H2a1 1 0 0 0 0 2h1a5.006 5.006 0 0 0 5-5V2a2 2 0 0 0-2-2Zm10 0h-4a2 2 0 0 0-2 2v4a2 2 0 0 0 2 2h4v1a3 3 0 0 1-3 3h-1a1 1 0 0 0 0 2h1a5.006 5.006 0 0 0 5-5V2a2 2 0 0 0-2-2Z"/>
                        </svg>
                        <blockquote>
                            <p class="text-xl italic font-medium text-slate-700 dark:text-white">"Every morning you have two choices: continue to sleep with your dreams, or wake up and chase them."</p>
                        </blockquote>
                        <figcaption class="flex items-center justify-center mt-6 space-x-3 rtl:space-x-reverse">
                            <div class="flex items-center divide-x-2 rtl:divide-x-reverse divide-gray-500 dark:divide-gray-700">
                                <cite class="pe-3 font-medium text-slate-500 dark:text-white">&#8212; Carmelo Anthony</cite>
                            </div>
                        </figcaption>
                    </figure>
                </section>

            </main>

            <!-- Footer -->
            <footer class="p-3 bg-white rounded-b-3xl">
                <p class="text-xs text-center tracking-widest">&copy; 2023 BTJ Academy </p>
            </footer>  
        
        </div>

    </div>
</template>

<script>
export default {
    methods: {
        doLogin() {
            navigateTo('/login')
            alert('Redirecting to Login Page')
        }
    }
}
</script>