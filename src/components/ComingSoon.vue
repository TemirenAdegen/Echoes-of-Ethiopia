<template>
  <div class="coming-soon-container">
    <img src="@/assets/hero-image.jpg" alt="Coming Soon Image" class="hero-image" />
    <div class="text-container">  
        <h1>Coming Soon</h1>
        <h1>በቅርብ ይመጣል</h1>
        </div>
  </div>
</template>

<script>
export default {
  name: "ComingSoon"
};
</script>

<style scoped>
.coming-soon-container {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: #fff;   /* white background */
  color: #000;              /* black text */
  font-family: 'Noto Sans Ethiopic', -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
    Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
  text-align: center;
  padding: 40px;
  gap: 40px;
}
.text-container {
  display: flex;
  flex-direction: column; 
  gap: 20px;
}

.hero-image {
  max-width: 50vw;
  max-height: 700%;
  height: auto;
  border-radius: 14px;
  user-select: none;
}

h1 {
  font-size: 5rem;
  font-weight: 700;
  letter-spacing: 0em;
  margin: 0;
  text-transform: uppercase;
  line-height: 1;
  text-shadow: none;
  box-shadow: none;
  font-style: italic;
}

/* Responsive styles for mobile */
@media (max-width: 600px) {
  .coming-soon-container {
    height: auto;
    flex-direction: column; /* stack image and text vertically */
    padding: 20px;
    gap: 20px;
  }

  .hero-image {
    max-width: 80vw;   /* larger image on smaller screens but fits inside */
    max-height: 60vh;
  }

  h1 {
    font-size: 3rem;   /* smaller font size */
    letter-spacing: 0.02em;  /* tighter spacing */
    text-align: center;
    font-style: italic;
  }
}
</style>