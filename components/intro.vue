<template>
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
</template>