<template>
  <div class="pt-28 css-selector md:h-screen ">
    <div class="px-4 md:px-28 md:py-14 py-6 mb-0 pb-0 text-center md:text-left">
      <div class="grid grid-cols-2 md:grid-cols-3 gap-4 md:pt-14">
        <div class="col-span-2">
          <h1
            class="font-bold text-6xl leading-tight"
            style="font-family: 'Poppins', sans-serif"
          >
            <span class="text-red-500">I</span>ndian
            <span class="text-red-500">S</span>ociety For <br /><span
              class="text-red-500"
              >T</span
            >echnical <span class="text-red-500">E</span>ducation
          </h1>
          <p class="text-xl pt-8 text-gray-700 pb-12">
            The Indian Society for Technical Education (ISTE) is the leading National Professional non-profit making Society for the Technical Education System.  
          </p>
          <button
            type="button"
            class="
              text-white
              bg-red-500
              hover:bg-red-400
              focus:outline-none focus:ring-4 focus:ring-red-300
              font-medium
              rounded-full
              text-base
              px-5
              py-2.5
              text-center
              mr-2
              mb-2
            "
          >
            Become a Member
          </button>
          <button
            class="
              text-white
              bg-gray-400
              hover:bg-gray-500
              focus:outline-none focus:ring-4 focus:ring-gray-300
              font-medium
              rounded-full
              text-base
              px-12
              py-2.5
              text-center
              mr-2
              mb-2
            "
          >
            Learn More
          </button>
        </div>
        <div class="flex items-center">
          <img
            id="content-desktop"
            class="
              animate__animated animate__pulse animate__slow animate__infinite
            "
            src="~/static/images/hero-img.svg"
            alt=""
          />
        </div>
      </div>
      <img
        id="content-mobile"
        class="
          py-5
          animate__animated animate__pulse animate__slow animate__infinite
        "
        src="~/static/images/hero-img.svg"
        alt=""
      />
      <br /><br />
      <a href="#About">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        id="content-desktop"
        width="40"
        height="40"
        viewBox="0 0 24 24"
        fill="none"
        stroke="#ef4444"
        stroke-width="2"
        stroke-linecap="round"
        stroke-linejoin="round"
        class="mx-auto feather feather-arrow-down-circle animate__animated animate__bounce animate__slow animate__infinite "
      >
        <circle cx="12" cy="12" r="10"></circle>
        <polyline points="8 12 12 16 16 12"></polyline>
        <line x1="12" y1="8" x2="12" y2="16"></line>
      </svg>
      </a>
    </div>
    <!-- <svg class="uvc-tilt-right-seperator" xmlns="http://www.w3.org/2000/svg" version="1.1" fill="rgb(248 113 113)" width="100%" height="100" viewBox="0 0 4 0.266661" preserveAspectRatio="none" style="height: 100px;"><polygon class="fil0" points="4,0 4,0.266661 -0,0.266661 "></polygon></svg> -->
  </div>
</template>

<script>
export default {};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@800&display=swap");

#content-desktop {
  display: block;
}
#content-mobile {
  display: none;
}
@media screen and (max-width: 768px) {
  #content-desktop {
    display: none;
  }
  #content-mobile {
    display: block;
  }
}

.css-selector {
  background: linear-gradient(-45deg, #97dbae, #c3e5ae, #f1e1a6, #f4bbbb);
  background-size: 400% 400%;
  animation: gradient 15s ease infinite;
}

@keyframes gradient {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}
</style>