<template>
  <div class="bg-[#292929] p-4 h-full min-h-screen">
    <h2 class="main-text-color text-center font-bold mt-4 mb-2 title dancing-script-font">
      Birthday Plan
    </h2>
    <p class="text-base font-normal main-text-color text-right">Thu, 11 Jul 2021</p>
    <div class="flex flex-col sm:grid grid-cols-19 mx-auto p-2 text-blue-50">
      <!-- left -->
      <div class="flex flex-row-reverse sm:contents mr-auto">
        <div class="col-start-1 col-end-10 rounded-xl my-4 text-left sm:text-right">
          <h3 class="text-lg font-semibold main-text-color">03:00 PM</h3>
          <p class="text-base font-normal main-text-color">Đi đón Mơ</p>
        </div>
        <div class="col-start-10 col-end-11 sm:mx-auto relative mr-4">
          <div class="h-full w-3 flex items-center justify-center">
            <div class="h-full w-0.5 bg-[#edece9] pointer-events-none"></div>
          </div>
          <div class="w-3 h-3 absolute top-1/2 -mt-3 rounded-full bg-[#edece9]"></div>
        </div>
      </div>
      <!-- right -->
      <div class="flex sm:contents">
        <div class="col-start-10 col-end-11 mr-4 sm:mx-auto relative">
          <div class="h-full w-3 flex items-center justify-center">
            <div class="h-full w-0.5 bg-[#edece9] pointer-events-none"></div>
          </div>
          <div class="w-3 h-3 absolute top-1/2 -mt-3 rounded-full bg-[#edece9]"></div>
        </div>
        <div class="col-start-11 col-end-20 rounded-xl my-4 mr-auto">
          <h3 class="text-lg font-semibold main-text-color">04:00 PM</h3>
          <p class="text-base font-normal main-text-color">Lấy bánh ở Amélie Cakery</p>
        </div>
      </div>
      <!-- left -->
      <div class="flex flex-row-reverse sm:contents mr-auto">
        <div class="col-start-1 col-end-10 rounded-xl my-4 text-left sm:text-right">
          <h3 class="text-lg font-semibold main-text-color">04:30 PM</h3>
          <p class="text-base font-normal main-text-color">Mua son Yves Saint Laurent Loveshine</p>
        </div>
        <div class="col-start-10 col-end-11 sm:mx-auto relative mr-4">
          <div class="h-full w-3 flex items-center justify-center">
            <div class="h-full w-0.5 bg-[#edece9] pointer-events-none"></div>
          </div>
          <div class="w-3 h-3 absolute top-1/2 -mt-3 rounded-full bg-[#edece9]"></div>
        </div>
      </div>
      <!-- right -->
      <div class="flex sm:contents">
        <div class="col-start-10 col-end-11 mr-4 sm:mx-auto relative">
          <div class="h-full w-3 flex items-center justify-center">
            <div class="h-full w-0.5 bg-[#edece9] pointer-events-none"></div>
          </div>
          <div class="w-3 h-3 absolute top-1/2 -mt-3 rounded-full bg-[#edece9]"></div>
        </div>
        <div class="col-start-11 col-end-20 rounded-xl my-4 mr-auto">
          <h3 class="text-lg font-semibold main-text-color">05:00 PM</h3>
          <p class="text-base font-normal main-text-color">Ăn tối ở Pizza 4P's Âu Cơ</p>
        </div>
      </div>
      <!-- left -->
      <div class="flex flex-row-reverse sm:contents mr-auto">
        <div class="col-start-1 col-end-10 rounded-xl my-4 text-left sm:text-right">
          <h3 class="text-lg font-semibold main-text-color">07:30 PM</h3>
          <p class="text-base font-normal main-text-color">Đưa Mơ về nhà</p>
        </div>
        <div class="col-start-10 col-end-11 sm:mx-auto relative mr-4">
          <div class="h-full w-3 flex items-center justify-center">
            <div class="h-full w-0.5 bg-[#edece9] pointer-events-none"></div>
          </div>
          <div class="w-3 h-3 absolute top-1/2 -mt-3 rounded-full bg-[#edece9]"></div>
        </div>
      </div>
    </div>
    <RouterLink to="/" class="block text-xs text-right text-slate-400 hover:underline">
      About us
    </RouterLink>
  </div>
</template>
<script setup></script>
<style>
.grid-cols-19 {
  grid-template-columns: repeat(19, minmax(0, 1fr));
}

.col-end-20 {
  grid-column-end: 20;
}

.main-text-color {
  color: #edece9;
}

.dancing-script-font {
  font-family: 'Dancing Script', cursive;
}

.title {
  font-size: 4.5rem;
  line-height: 1.15;
}

p,
h3 {
  font-family: Montserrat;
  letter-spacing: 0.1em;
}
</style>
