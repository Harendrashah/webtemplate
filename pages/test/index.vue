<template>
    <div>
        <div class="h-[100vh] bg-red-200">asd</div>
      <!-- Parallax Section with YouTube iframe -->
      <div class="parallax-wrapper">
        <iframe
          src="https://www.youtube.com/embed/CQEPHM_tuYw?si=qRtDnP7ZzqrJVJRm"
          frameborder="0"
          class="parallax-iframe"
        ></iframe>
        <div class="overlay-content">
          <h1 class="text-center text-white text-4xl">First Section</h1>
        </div>
      </div>
  
      <!-- Static Content Section -->
      <div class="content-section">
        <h1 class="text-center text-black text-4xl">Second Section</h1>
      </div>
    </div>
  </template>
  
  <style scoped>
  /* Wrapper for Parallax Section */
  .parallax-wrapper {
    position: relative;
    height: 100vh;
    overflow: hidden;
  }
  
  /* Parallax Iframe */
  .parallax-iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 150%; /* Make it larger to emphasize parallax */
    z-index: -1;
    transform: translateY(-20%); /* Initial offset */
    transition: transform 0.2s linear; /* Smooth effect on scroll */
    pointer-events: none; /* Disable interaction */
  }
  
  /* Overlay Content */
  .overlay-content {
    position: relative;
    z-index: 10;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    background: rgba(0, 0, 0, 0.4); /* Optional dark overlay for contrast */
  }
  
  /* Static Content Section */
  .content-section {
    height: 100vh;
    background-color: #f8f9fa;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
  /* Parallax Effect using JavaScript */
  </style>
  
  <script>
  export default {
    mounted() {
      const iframe = document.querySelector('.parallax-iframe');
      window.addEventListener('scroll', () => {
        const scrollPosition = window.scrollY;
        iframe.style.transform = `translateY(${scrollPosition * -0.2}px)`; // Adjust speed by changing multiplier
      });
    },
  };
  </script>
  