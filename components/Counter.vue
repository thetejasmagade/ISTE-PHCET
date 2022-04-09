<template>
<div>
  <div class="mt-8" style="background-color: #212121">
    <div class="md:mx-32 mx-8">
      <div class="grid grid-cols-2 md:grid-cols-4 gap-1 text-center py-12">
        <div class="">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="84"
            height="84"
            viewBox="0 0 24 24"
            fill="none"
            stroke="#ef4444"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
            class="feather feather-users mx-auto mb-3"
          >
            <path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"></path>
            <circle cx="9" cy="7" r="4"></circle>
            <path d="M23 21v-2a4 4 0 0 0-3-3.87"></path>
            <path d="M16 3.13a4 4 0 0 1 0 7.75"></path>
          </svg>
          <number
            class="md:text-5xl text-2xl font-extrabold text-white pt-8"
            style='Inter, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif;'
            ref="number4"
            :from="0"
            :to="100"
            :format="theFormat"
            :duration="2"
            :delay="2"
            easing="Power1.easeOut"
          />
          <h2
            class="md:text-3xl font-bold text-white pt-2"
            style='Inter, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif;'
          >
            MEMBERS
          </h2>
        </div>
        <div class="...">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="84"
            height="84"
            viewBox="0 0 24 24"
            fill="none"
            stroke="#ef4444"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
            class="feather feather-calendar mx-auto mb-3"
          >
            <rect x="3" y="4" width="18" height="18" rx="2" ry="2"></rect>
            <line x1="16" y1="2" x2="16" y2="6"></line>
            <line x1="8" y1="2" x2="8" y2="6"></line>
            <line x1="3" y1="10" x2="21" y2="10"></line>
          </svg>
          <number
            class="md:text-5xl text-2xl font-extrabold text-white pt-8"
            style='Inter, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif;'
            ref="number3"
            :from="0"
            :to="30"
            :format="theFormat"
            :duration="2"
            :delay="2"
            easing="Power1.easeOut"
          />
          <h2
            class="md:text-3xl font-bold text-white pt-2"
            style='Inter, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif;'
          >
            EVENTS
          </h2>
        </div>
        <div class="pt-12 md:pt-0">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="84"
            height="84"
            viewBox="0 0 24 24"
            fill="none"
            stroke="#ef4444"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
            class="feather feather-anchor mx-auto mb-3"
          >
            <circle cx="12" cy="5" r="3"></circle>
            <line x1="12" y1="22" x2="12" y2="8"></line>
            <path d="M5 12H2a10 10 0 0 0 20 0h-3"></path>
          </svg>
          <number
            class="md:text-5xl text-2xl font-extrabold text-white pt-8"
            style='Inter, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif;'
            ref="number2"
            :from="0"
            :to="100"
            :format="theFormat"
            :duration="2"
            :delay="2"
            easing="Power1.easeOut"
          />
          <h2
            class="md:text-3xl font-bold text-white pt-2"
            style='Inter, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif;'
          >
            WORKSHOPS
          </h2>
        </div>
        <div class="pt-12 md:pt-0">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="84"
            height="84"
            viewBox="0 0 24 24"
            fill="none"
            stroke="#ef4444"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
            class="feather feather-user mx-auto mb-3"
          >
            <path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path>
            <circle cx="12" cy="7" r="4"></circle>
          </svg>
          <number
            class="md:text-5xl text-2xl font-extrabold text-white pt-8"
            style='Inter, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif;'
            ref="number1"
            :from="0"
            :to="250"
            :format="theFormat"
            :duration="2"
            :delay="2"
            easing="Power1.easeOut"
          />
          <h2
            class="md:text-3xl font-bold text-white pt-2"
            style='Inter, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif;'
          >
            PARTICIPANTS
          </h2>
        </div>
      </div>
    </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>