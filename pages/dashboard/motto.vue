<template>
    <div class="flex min-h-screen text-gray-700 bg-custom-bg">

    <!-- MAIN CONTAINER -->
    <div class="container m-auto w-5/6 shadow-2xl bg-white rounded-2xl overflow-auto h-[90vh]">
        <CmsHeader />

        <main class="flex h-screen">
            <aside class="w-1/5 space-y-8 text-center p-5 bg-blue-300">
                <p class="text-xl hover:font-bold"><NuxtLink to="/dashboard"> Introduction</NuxtLink></p>
                <p class="text-xl hover:font-bold"><NuxtLink to="/dashboard/education">Education</NuxtLink></p>
                <p class="text-xl hover:font-bold"><NuxtLink to="/dashboard/work"> Work Experiences </NuxtLink></p>
                <p class="text-xl font-bold hover:font-bold"><NuxtLink to="/dashboard/motto"> Motto </NuxtLink></p>
                <p class="text-xl hover:font-bold"><NuxtLink to="/dashboard/contact"> Contact </NuxtLink></p>
            </aside>
          <section class="w-4/5 p-5">
             <div class="flex items-center justify-between">
                <h1 class="text-2xl font-semibold">Motto</h1>
                <button class="bg-blue-500 hover:bg-blue-800 px-5 py-1 rounded-md text-gray-100 tracking-wide">Edit</button>
             </div>

              <MottoEdit />
          </section>
        </main>

        <CmsFooter />
    </div>
  </div>
</template>

<script>
definePageMeta({
  layout:'cmsLayout'
})

</script>