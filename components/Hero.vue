<template>
  <!-- <div class="pt-28 css-selector md:h-screen ">
    <div class="px-4 md:px-28 md:py-14 py-6 mb-0 pb-0 text-center md:text-left">
      <div class="grid grid-cols-2 md:grid-cols-3 gap-4 md:pt-14">
        <div class="col-span-2">
          <h1
            class="font-bold text-6xl leading-tight"
            style="font-family: 'Poppins', sans-serif"
          >
            <span class="text-red-500">I</span>STE - <span class="text-red-500">P</span>HCET
          </h1>
          <p class="text-xl pt-8 text-gray-700 pb-12">
            Empowering the future by technology  
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
  </div> -->
  <header
    id="up"
    class="bg-center bg-fixed bg-no-repeat bg-center bg-cover h-screen relative"
  >
    <!-- Overlay Background + Center Control -->
    <div
      class="h-screen bg-opacity-50 bg-black flex items-center justify-center"
      style="background: rgba(0, 0, 0, 0.8)"
    >
      <div class="mx-2 text-center">
        <h1
          class="font-bold md:text-6xl text-5xl leading-tight text-white"
          style="font-family: 'Poppins', sans-serif"
        >
          ISTE <span class="text-red-500">X</span>
          <span
            class="txt-rotate"
            data-period="2000"
            data-rotate='[ "PHCET" ]'
          ></span>
        </h1>
        <p class="text-xl pt-8 text-gray-100 pb-12">
          Empowering the future by technology
        </p>
        <div class="inline-flex">
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
      </div>
    </div>
  </header>
</template>

<script>
var TxtRotate = function (el, toRotate, period) {
  this.toRotate = toRotate;
  this.el = el;
  this.loopNum = 0;
  this.period = parseInt(period, 10) || 2000;
  this.txt = "";
  this.tick();
  this.isDeleting = false;
};

TxtRotate.prototype.tick = function () {
  var i = this.loopNum % this.toRotate.length;
  var fullTxt = this.toRotate[i];

  if (this.isDeleting) {
    this.txt = fullTxt.substring(0, this.txt.length - 1);
  } else {
    this.txt = fullTxt.substring(0, this.txt.length + 1);
  }

  this.el.innerHTML = '<span class="wrap">' + this.txt + "</span>";

  var that = this;
  var delta = 300 - Math.random() * 100;

  if (this.isDeleting) {
    delta /= 2;
  }

  if (!this.isDeleting && this.txt === fullTxt) {
    delta = this.period;
    this.isDeleting = true;
  } else if (this.isDeleting && this.txt === "") {
    this.isDeleting = false;
    this.loopNum++;
    delta = 500;
  }

  setTimeout(function () {
    that.tick();
  }, delta);
};

window.onload = function () {
  var elements = document.getElementsByClassName("txt-rotate");
  for (var i = 0; i < elements.length; i++) {
    var toRotate = elements[i].getAttribute("data-rotate");
    var period = elements[i].getAttribute("data-period");
    if (toRotate) {
      new TxtRotate(elements[i], JSON.parse(toRotate), period);
    }
  }
  // INJECT CSS
  var css = document.createElement("style");
  css.type = "text/css";
  css.innerHTML = ".txt-rotate > .wrap { border-right: 0.08em solid #ef4444 }";
  document.body.appendChild(css);
};
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

header {
  background: url("~/static/herobg.jpg");
}
</style>