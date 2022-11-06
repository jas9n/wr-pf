<template>
    <div id="projects">
        <global-navbar />
        <section class="min-h-screen w-full flex justify-center items-center pt-32 pb-12 px-12">
            <div id="container" class="w-full overflow-visible grid grid-cols-1 grid-flow-row justify-items-center place-content-center gap-2 md:grid-cols-2 lg:grid-cols-3">
                <client-profile/>
                <client-profile/>
                <client-profile/>
                <client-profile/>
            </div>
        </section>
        <global-footer/>
    </div>
</template>

<script>
export default {
    name: "Projects"
}
</script>