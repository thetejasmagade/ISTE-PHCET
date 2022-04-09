<template>
  <div>
    <NuxtLink to="/">
      <!-- <a
        class="text-black font-bold text-3xl"
        style="font-family: 'Monoton', cursive"
        ><span class="text-red-500">ISTE</span>&nbsp; PHCET</a
      > -->
      <!-- <img src="~/static/images/logo.png" height="50" width="50"> -->
      <div class="row">
        <div class="column">
          <img src="~/static/images/logo.png" style="width: 50%" />
        </div>
        <div class="column" id="content-desktop">
          <img src="https://storage.googleapis.com/ezap-prod/colleges/1817/pillai-hoc-college-of-engineering-and-technology-khalapur-logo.jpg" style="width: 25%" />
        </div>
      </div>
    </NuxtLink>
  </div>
</template>

<script>
export default {};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Monoton&display=swap");

.column {
  float: left;
  /* width: 33.33%; */
  /* padding: 3px; */
}

/* Clear floats after image containers */
.row::after {
  content: "";
  clear: both;
  display: table;
}
</style>