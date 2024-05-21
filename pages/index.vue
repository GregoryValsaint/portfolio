<script setup>
const { data: posts } =await useAsyncData('latest-posts', () =>
    queryContent('/blog')
        .sort({ data:1 })
        .limit(3)
        .find()
)
</script>

<template>
    <!---MYSELF-->
    <section>
        <h1 class="text-5xl font-bold mt-20">👋🏻 Salut, Je suis Grégory Valsaint!</h1>
        <p class="text-base text-gray-900 p-2 italic">Developpeur Fullstack Vue.js </p>
    </section>

    <!---sTORY-->
    <section class="flex flex-col md:flex-row">
        <div class="md:w-3/4">
        <h2 class="text-4xl text-gray-900 font-bold mt-8">My Story</h2>
        <p class="text-lg py-2">
            Développeur Fullstack Vue.js passionné, je suis à la recherche de nouveaux challenges.
            J'ai obtenu un Bac +3 en tant que responsable en ingénierie des logiciels et j'ai acquis une solide expérience en JavaScript, HTML/CSS et Vue.js. 
            Je suis capable de réaliser des applications web complètes, du design front-end à l'architecture back-end et de manager, collaborer à l’étude préalable des projets IT.
        </p>
        <p class="text-lg py-2">
            Rigoureux et méthodique, je suis capable de travailler de manière autonome et en équipe. 
            Je suis également doté d'excellentes capacités de communication et de résolution de problèmes.
        </p>
        <p class="text-lg py-2">
            Je suis convaincu que mes compétences et mon expérience feront de moi un atout précieux pour votre équipe. 
            Je suis très motivé à l'idée de rejoindre une entreprise innovante et dynamique comme la vôtre et de contribuer à son développement.
        </p>
        </div>
        <img src="https://fly.storage.tigris.dev/sticker-bucket/prediction-94259-sticker.png" class="w-1/2 md:max-w-sm p-8 mx-auto" />
    </section>

    <!---HARD SKILLS-->
    <section >
        <p class="text text-red-500 font-bold mt-8 text-center">Hard Skills</p>
        <h2 class="text-4xl text-gray-900 font-bold  text-center">Hard Skills</h2>
        <div class="grid grid-cols-2 gap-4 mt-8">
            <!---row 1-->
            <div>
                <div class="bg-white max-w-sm mx-auto rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl transition duration-500 transform hover:scale-105 cursor-pointer">
                    <div class="h-20 bg-red-500 flex items-center justify-between">
                        <h1 class="text-white ml-4 border-2 py-2 px-4 rounded-full">1</h1>
                        <p class="mr-20 text-white text-lg">HTML/CSS</p>
                        <p class="mr-4 text-white font-thin text-lg">90 %</p>
                    </div>

                    <p class="py-6 text-lg tracking-wide ml-16">Description of what is done here</p>
                    <!-- <hr > -->
                    <div class="flex justify-between px-5 mb-2 text-sm text-gray-600">
                        <p>Last Update</p>
                        <p>3/08/2021</p>
                    </div>
                </div>
            </div>
            <div>
                <div class="bg-white max-w-sm mx-auto rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl transition duration-500 transform hover:scale-105 cursor-pointer">
                    <div class="h-20 bg-red-500 flex items-center justify-between">
                        <h1 class="text-white ml-4 border-2 py-2 px-4 rounded-full">2</h1>
                        <p class="mr-20 text-white text-lg">Javascript</p>
                        <p class="mr-4 text-white font-thin text-lg">85 %</p>
                    </div>

                    <p class="py-6 text-lg tracking-wide ml-16">Description of what is done here</p>
                    
                    <!-- <hr > -->
                    <div class="flex justify-between px-5 mb-2 text-sm text-gray-600">
                        <p>Last Update</p>
                        <p>3/08/2021</p>
                    </div>
                </div>
            </div>
            <!---row 2-->
            <div>
                <div class="bg-white max-w-sm mx-auto rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl transition duration-500 transform hover:scale-105 cursor-pointer">
                    <div class="h-20 bg-red-500 flex items-center justify-between">
                        <h1 class="text-white ml-4 border-2 py-2 px-4 rounded-full">3</h1>
                        <p class="mr-20 text-white text-lg">Vue.JS/Nuxt</p>
                        <p class="mr-4 text-white font-thin text-lg">90 %</p>
                    </div>

                    <p class="py-6 text-lg tracking-wide ml-16">Description of what is done here</p>
                    <!-- <hr > -->
                    <div class="flex justify-between px-5 mb-2 text-sm text-gray-600">
                        <p>Last Update</p>
                        <p>3/08/2021</p>
                    </div>
                </div>
            </div>
            <div>
                <div class="bg-white max-w-sm mx-auto rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl transition duration-500 transform hover:scale-105 cursor-pointer">
                    <div class="h-20 bg-red-500 flex items-center justify-between">
                        <h1 class="text-white ml-4 border-2 py-2 px-4 rounded-full">4</h1>
                        <p class="mr-20 text-white text-lg">Flutter</p>
                        <p class="mr-4 text-white font-thin text-lg">75 %</p>
                    </div>

                    <p class="py-6 text-lg tracking-wide ml-16">Description of what is done here</p>
                    
                    <!-- <hr > -->
                    <div class="flex justify-between px-5 mb-2 text-sm text-gray-600">
                        <p>Last Update</p>
                        <p>3/08/2021</p>
                    </div>
                </div>
            </div>
            <!---row 3-->
            <div>
                <div class="bg-white max-w-sm mx-auto rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl transition duration-500 transform hover:scale-105 cursor-pointer">
                    <div class="h-20 bg-red-500 flex items-center justify-between">
                        <h1 class="text-white ml-4 border-2 py-2 px-4 rounded-full">5</h1>
                        <p class="mr-20 text-white text-lg">Python/Django</p>
                        <p class="mr-4 text-white font-thin text-lg">85%</p>
                    </div>

                    <p class="py-6 text-lg tracking-wide ml-16">Description of what is done here</p>
                    <!-- <hr > -->
                    <div class="flex justify-between px-5 mb-2 text-sm text-gray-600">
                        <p>Last Update</p>
                        <p>3/08/2021</p>
                    </div>
                </div>
            </div>
            <div>
                <div class="bg-white max-w-sm mx-auto rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl transition duration-500 transform hover:scale-105 cursor-pointer">
                    <div class="h-20 bg-red-500 flex items-center justify-between">
                        <h1 class="text-white ml-4 border-2 py-2 px-4 rounded-full">6</h1>
                        <p class="mr-20 text-white text-lg">Git</p>
                        <p class="mr-4 text-white font-thin text-lg">90%</p>
                    </div>

                    <p class="py-6 text-lg tracking-wide ml-16">Description of what is done here</p>
                    
                    <!-- <hr > -->
                    <div class="flex justify-between px-5 mb-2 text-sm text-gray-600">
                        <p>Last Update</p>
                        <p>3/08/2021</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!---PROJECT-->

    <!---BLOG-->
    <section>
        <h2 class="text-4xl font-bold mt-8 text-center">Derniers articles</h2>
        <div class="grid md:grid-cols-3 pt-8 mb-8 gap-10">
            <Post :posts="posts" />
        </div>
    </section>
</template>

