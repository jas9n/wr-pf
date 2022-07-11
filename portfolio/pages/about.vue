<template>
    <div id="about">
        <global-navbar />
        <section id="info" class="h-auto min-h-screen w-full flex flex-col justify-center items-center space-y-6 pt-20 md:pt-4">
            <h2 class="w-3/4 text-white text-5xl text-center font-medium overflow-visible">We are WebRising.</h2>
            <div id="content" class="h-auto w-3/4 flex flex-col justify-center items-center space-y-6 md:flex-row md:items-start md:space-y-0 md:space-x-12 lg:w-2/3 ">
                <div id="divider" class="w-full h-full flex flex-col justify-start items-start space-y-6 text-white font-medium text-lg md:w-1/2">
                    <p>WebRising is a <span class="text-rose-300"> non-profit </span> organization that connects volunteer
                    <span class="text-rose-300"> high school developers </span> to <span class="text-rose-300"> small local businesses </span> in need of a web-based platform to market their business, completely <span class="text-rose-300"> free of charge</span>.</p>
                    <p>We seek to help small businesses navigate the advent of web-based
                    platforms while <span class="text-rose-300"> empowering volunteers </span> with real-world experience
                    and promoting a greater sense of <span class="text-rose-300"> community</span>.</p>
                </div>
                <div id="divider" class="w-full h-full flex flex-col justify-start items-start space-y-6 text-white font-medium text-lg md:w-1/2">
                    <p>Whether you need a static website to simply <span class="text-rose-300"> showcase your business </span>
                    and display important information, or a platform to <span class="text-rose-300"> expedite sales </span>
                    — <span class="text-rose-300"> we've got you covered</span>. Our team has the resources and technical
                    expertise to craft a streamlined platform.
                    </p>
                    <p>Let's create something<span class="text-rose-300"> awesome</span>!</p>
                </div>
            </div>
        </section>
        <section id="team" class="h-auto min-h-screen w-full flex flex-col justify-center items-center">
            <h2 class="w-3/4 text-white text-5xl text-center font-medium overflow-visible">Our team.</h2>
            <div id="content" class="h-auto w-3/4 flex flex-col justify-center items-center">
                
            </div>

        </section>
        <global-footer/>
    </div>
</template>

<script>
export default {
    name: "About"
}
</script>