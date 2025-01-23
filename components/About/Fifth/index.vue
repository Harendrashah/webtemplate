<template>
    <div class="flex flex-col justify-center items-center h-[100vh] mt-8">
      <img src="../../../assets/icons/user.svg" alt="usericon" class="mt-8" />
  
      <div class="flex flex-col items-center mt-5">
        <span class="text-[36px] md:w-[569px] text-[#353F53] font-bold text-center">
          Save your time and money by choosing our professional team.
        </span>
      </div>
  
     <div class="flex flex-col md:flex-row">
       <!-- User Cards Carousel -->
       <UCarousel v-slot="{ item }" :items="userCards">
        <AboutUserCard
          :name="item.name"
          :title="item.title"
          :profileImage="item.profileImage"
          :description="item.description"
        />
        
      </UCarousel>
     </div>
    </div>
  </template>
  
  <script setup>
  import blackigga from '../../../assets/icons/blacknigga.svg'
  import image1 from '../../../assets/images/bg12.jpg'
  
  
 
  const userCards = [
    {
      name: "Alice Johnson",
      title: "Frontend Developer",
      profileImage: blackigga,
      description: "Creative and passionate frontend developer with 5 years of experience.",
    },
    {
      name: "Bob Smith",
      title: "Backend Developer",
      profileImage: image1,
      description: "Experienced backend developer specializing in database management.",
    },
    {
      name: "Charlie Davis",
      title: "UI/UX Designer",
      profileImage: image1,
      description: "UI/UX designer with a focus on user-centered design and interactive experiences.",
    },
    
    {
      name: "Diana Williams",
      title: "Project Manager",
      profileImage: image1,
      description: "Project manager with strong organizational skills and proven leadership abilities.",
    },
  
    
  ];
  </script>
  
  <style>
  
  </style>
  