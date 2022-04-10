<template>
  <div>
    <Navbar />
    <PagesHero pageName="Gallery" />
    <div id="main"></div>
    <h1
      class="
        text-5xl
        font-extrabold
        text-transparent
        bg-clip-text bg-gradient-to-br
        from-yellow-400
        to-red-600
        pt-5
        text-center
        py-2
      "
      style='Inter, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif;'
    >
      Gallery
    </h1>
    <section class="overflow-hidden text-gray-700">
      <div class="container px-5 py-12 mx-auto lg:px-32">
        <div class="flex flex-wrap -m-1 md:-m-2">
          <div class="flex flex-wrap w-1/2">
            <div class="w-full p-1 md:p-2">
              <img
                alt="gallery"
                class="
                  block
                  object-cover object-center
                  w-full
                  h-full
                  rounded-lg
                "
                src="~/static/poster1.jpg"
              />
            </div>
          </div>
          <div class="flex flex-wrap w-1/2">
            <div class="w-full p-1 md:p-2">
              <img
                alt="gallery"
                class="
                  block
                  object-cover object-center
                  w-full
                  h-full
                  rounded-lg
                "
                src="~/static/poster2.png"
              />
            </div>
          </div>
        </div>
      </div>
    </section>

    <Footer />
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>