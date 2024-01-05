<template>
    <form class="grid space-y-3 mt-5">
        <label for="fullname">Full Name</label>
        <input type="text" id="fullname" placeholder="Enter full name here" value="Nur Fadhilah Sadrah">
        <label for="profileDescription">Profile Description</label>
        <textarea type="text" id="profileDescription" rows="5" placeholder="Enter description about yourself here">Informatics Engineering graduate and passionate Software Developer. With a keen eye for design and a knack for coding, I bring ideas to life by building visually stunning and highly functional web & mobile apps. I'm also interested in AI and Machine Learning. In my free time, I enjoy listening to music, reading webtoons, fangirling, and watching variety shows.</textarea>
        <label for="profilePicture">Profile Picture</label>
        <input type="file" id="profilePicture">
        <button class="bg-blue-600 hover:bg-blue-800 px-5 py-2 rounded-md text-gray-100 tracking-wide">SAVE</button>
    </form>
</template>