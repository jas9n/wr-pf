<template>
    <div id="client">
        <div id="content" class="flex justify-center items-center cursor-pointer group border border-black rounded-sm">
            <div class="w-full h-full aspect-square object-cover overflow-hidden ease-in duration-200 group-hover:scale-110">
                <img src="https://images.unsplash.com/photo-1657397658615-5334c00cac92?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1472&q=80" alt="">
            </div>
            <div id="overlay" class="absolute flex flex-col justify-center z-10 items-center space-y-1">
                <div class="absolute w-full h-full bg-black opacity-0 -z-10 ease-in duration-200 group-hover:opacity-60"></div>
                <div class="text-white ease-in duration-200 opacity-0 group-hover:opacity-100">
                    <h3 class="text-2xl font-medium">Client</h3>
                    <h4 class="text-lg">Details</h4>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "Client",
}
</script>

<style scoped>
#content {
    width: 90vw;
    height: auto;
    aspect-ratio: 1/1;
}
#overlay {
    width: 90vw;
    height: auto;
    aspect-ratio: 1/1;
}

@media (min-width: 640px) {
    #content {
        width: 45vw;
        height: auto;
        aspect-ratio: 1/1;
    }
    #overlay {
        width: 45vw;
        height: auto;
        aspect-ratio: 1/1;
    }
}
@media (min-width: 768px) {
    #content {
        width: 45vw;
        height: auto;
        aspect-ratio: 1/1;
    }
    #overlay {
        width: 45vw;
        height: auto;
        aspect-ratio: 1/1;
    }
}
@media (min-width: 1024px) {
    #content {
        width: 30vw;
        height: auto;
        aspect-ratio: 1/1;
    }
    #overlay {
        width: 30vw;
        height: auto;
        aspect-ratio: 1/1;
    }
}
</style>