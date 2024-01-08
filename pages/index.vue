<template>
  <div class="text-center mt-20">
    <div class="text-9xl font-bold mb-6 animate__animated animate__fadeInUp">
      Hi, I'm AD
    </div>
    <div class="text-9xl font-bold mb-6 border-text animate__animated animate__fadeInUp">
      Hi, I'm AD
    </div>
    <div class="text-9xl font-bold mb-6 animate__animated animate__fadeInUp">
      Hi, I'm AD
    </div>
  </div>
</template>

<style scoped>
  /* Add this link to your HTML head for animate.css styles */
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

  .animate__animated {
    animation-duration: 0.2s; /* Adjust the duration as needed */
    animation-fill-mode: both;
    animation-timing-function: ease-out; /* Use ease-out for a quicker appearance */
  }

  .animate__delay-1s {
    animation-delay: 0.5s; /* Adjust the delay as needed */
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
