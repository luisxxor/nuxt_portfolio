<template>
  <section id="aboutMeInfoSection" class="flex w-screen h-screen px-8">
    <div id="aboutMePatternBackground"></div>
    <div class="container mx-auto">
      <article id="aboutMeInfoArticle" class="flex flex-wrap h-full py-8">
        <h1 class="text-white text-center sm:text-3xl md:text-4xl">Hello! my name is Luis Portillo</h1>
        <p class="text-white mt-10 text-justify sm:text-md md:text-xl">
          I'm a 21 years old fullstack web developer that loves coding and learning something new every day. 
<strike> Although it sounds cliché</strike> I like the challenges that allow me to overcome and at the same time be able to create cool things.
          <br>
          <br>If you continue scrolling, you can see some projects that I have developed.
        </p>

        <img
          src="~assets/avatar.jpg"
          alt="Luis Portillo"
          class="w-64 h-64 rounded-lg mx-auto mt-auto"
        >
      </article>
    </div>
  </section>
</template>

<style>
#aboutMeInfoSection {
  position: relative;
}

#aboutMePatternBackground {
  background-color: #000000;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' height='32' viewBox='0 0 16 32'%3E%3Cg fill='%23222222' fill-opacity='0.4'%3E%3Cpath fill-rule='evenodd' d='M0 24h4v2H0v-2zm0 4h6v2H0v-2zm0-8h2v2H0v-2zM0 0h4v2H0V0zm0 4h2v2H0V4zm16 20h-6v2h6v-2zm0 4H8v2h8v-2zm0-8h-4v2h4v-2zm0-20h-6v2h6V0zm0 4h-4v2h4V4zm-2 12h2v2h-2v-2zm0-8h2v2h-2V8zM2 8h10v2H2V8zm0 8h10v2H2v-2zm-2-4h14v2H0v-2zm4-8h6v2H4V4zm0 16h6v2H4v-2zM6 0h2v2H6V0zm0 24h2v2H6v-2z'/%3E%3C/g%3E%3C/svg%3E");
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  z-index: -1;
}

#aboutMeInfoArticle > h1 {
  flex: 1 0 100%;
}

#aboutMeTitleInfo {
  color: #000f08;
}
</style>
