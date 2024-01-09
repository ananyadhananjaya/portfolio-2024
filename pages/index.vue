<template>
  <div class="text-center mt-20">
    <div
      class="text-9xl font-bold mb-6 animate__animated animate__delay-1s animate__fadeInUp"
    >
      Hi, I'm AD
    </div>
    <div
      class="text-9xl font-bold mb-6 border-text animate__delay-1s animate__animated animate__fadeInUp"
    >
      Hi, I'm AD
    </div>
    <div
      class="text-9xl font-bold mb-6 animate__animated animate__delay-1s animate__fadeInUp"
    >
      Hi, I'm AD
    </div>
  </div>
  <div
    class="absolute bottom-12 right-0 flex flex-col items-center justify-center space-y-8"
  >
    <div class="rotate-90 text-body-3">scroll</div>
    <div style="height: 60px">
      <div class="scroll__element animate_scroll_slide"></div>
    </div>
  </div>
</template>

<style scoped>
@keyframes fadeInUp {
  0% {
    opacity: 0;
    transform: scaleY(0);
    transform-origin: bottom;
  }
  100% {
    opacity: 1;
    transform: scaleY(1);
    transform-origin: bottom;
  }
}

@keyframes slide {
  0% {
    transform: translate3d(0px);
    height: 40px;
  }
  100% {
    height: 0px;
    transform: translateY(40px); 
  }
}

.scroll__element {
  height: 60px;
  width: 1px;
  color: black;
}

.animate_scroll_slide {
  background-color: black;
  animation: slide 1s infinite;
  animation-timing-function: ease-in;
}

.animate__animated {
  animation-duration: 0.4s; 
  animation-fill-mode: both;
  animation-timing-function: ease-out; 
}

.animate__delay-1s {
  animation-delay: 0.5s; 
}

.animate__fadeInUp {
  animation-name: fadeInUp;
}

/* Style for text with only borders */
.border-text {
  -webkit-text-stroke: 2px #618264;
  color: transparent;
}
</style>
