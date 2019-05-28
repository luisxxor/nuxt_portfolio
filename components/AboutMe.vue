<template>
  <section id="aboutMeSection" class="flex align-center justify-center w-screen h-screen">
    <div id="backgroundImage"></div>
    <h1 id="aboutMeTitle" class="text-center sm:text-4xl md:text-5xl my-auto">
      I'm Luis Portillo
      <br>a Fullstack Developer
    </h1>
    <svg id="arrow" viewBox="0 0 20 20" class="fill-current text-white inline-block h-12 w-12">
      <path d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"></path>
    </svg>
  </section>
</template>

<style>
#arrow {
  bottom: 5px;
  left: calc(50vw - 1.5rem);
  position: absolute;
  animation: arrowFloating 2s infinite ease-in-out;
  cursor: pointer;
}

#backgroundImage {
  background-image: url(~assets/laptopbackground500.jpg);
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
  position: absolute;
  top: 0;
  bottom: 0;
  right: 0;
  left: 0;
  z-index: -1;
  filter: brightness(60%) contrast(110%);
}

#aboutMeTitle {
  color: #e2e2e2;
  text-transform: capitalize;
}

@media only screen and (min-width: 501px) {
  #backgroundImage {
    background-image: url(~assets/laptopbackground1280.jpg);
  }
}
@media only screen and (min-width: 1281px) {
  #backgroundImage {
    background-image: url(~assets/laptopbackground1900.jpg);
  }
}

@media only screen and (min-width: 1901px) {
  #backgroundImage {
    background-image: url(~assets/laptopbackground.jpg);
  }
}

@keyframes arrowFloating {
  0% {
    transform: translateY(0);
  }

  50% {
    transform: translateY(6px);
  }

  100% {
    transform: translateY(0);
  }
}
</style>
