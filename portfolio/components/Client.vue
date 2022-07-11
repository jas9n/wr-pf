<template>
    <div id="project">
        <div id="content" class="w-80 h-80 flex justify-center items-center cursor-pointer group border border-black rounded-sm sm:w-96 sm:h-96 md:w-80 md:h-80 lg:w-96 lg:h-96">
            <div class="w-full h-full aspect-square object-cover overflow-hidden ease-in duration-200 group-hover:scale-110">
                <img src="https://images.unsplash.com/photo-1657397658615-5334c00cac92?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1472&q=80" alt="">
            </div>
            <div id="overlay" class="absolute w-80 h-80 flex flex-col justify-center z-10 items-center space-y-1 sm:w-96 sm:h-96 md:w-80 md:h-80 lg:w-96 lg:h-96">
                <div class="absolute w-full h-full bg-black opacity-0 -z-10 ease-in duration-200 group-hover:opacity-60"></div>
                <div class="text-white ease-in duration-200 opacity-0 group-hover:opacity-100">
                    <h3 class="text-2xl font-medium">Client</h3>
                    <h4 class="text-lg">Details</h4>
                </div>
            </div>
        </div>
    </div>
</template>