<script>
  import Card from './lib/Card.svelte'
  import Button from "./lib/Button.svelte"
  // import ImageHero from "./assets/image-hero-desktop@2x.webp"
</script>

<!-- <Counter /> -->
<div class="container">
  <header>
    <img src="/assets/logo-dark.svg" alt="skilled" class="logo"/>
    <Button type="blue"/>
  </header>
  <main>  
    <div class="hero">
      <div class="hero-card">
        <h1>
          Maximize skill,<br /> minimize budget
        </h1>
        <p>
          Our modern courses across a range of in-demand skills will give you the 
          knowledge you need to live the life you want.
        </p> 
        <Button type="red" big={true}/>
      </div>
      <img src="/assets/image-hero-desktop.webp" alt="hero" class="hero-image"/>
    </div>
    <div class="cards">
      <div class="single-card">
        <h2 class="check-out">Check out our most popular courses!</h2>
      </div>
      <Card title="Animation" text="Learn the latest animation techniques to create stunning motion 
      design and captivate your audience." icon="icon-animation"  />
      
      <Card title="Design" text="Create beautiful, usable interfaces to help shape the future of 
      how the web looks." icon="icon-design"  />
      
      <Card title="Photography" text="Explore critical fundamentals like lighting, composition, and focus 
      to capture exceptional photos." icon="icon-photography"  />
    
    <Card title="Crypto" text="All you need to know to get started investing in crypto. Go from beginner 
    to advanced with this 54 hour course." icon="icon-crypto" />
    
    <Card title="Business" text="A step-by-step playbook to help you start, scale, and sustain your business 
    without outside investment." icon="icon-business" />
  </div>
  </main>
</div>
    <footer>
      <img src="/assets/logo-light.svg" alt="skilled" class="logo" />
      <Button type="purple" />
    </footer>


<style>
  header, footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  header {
    margin-top: 24px;
  }

  footer {
    height: 120px;
    padding: 32px 165px;
    background-color: var(--dark-blue);
    position: absolute;
    width: 100%;
    bottom: 0
  }

  .hero {
    display: flex;
  }

  .hero-card {
    /* width: 50%; */
    width: 457px;
    margin: 172px 162px 226px 0px;
  }

  .hero-image {
    /* width: 50%; */
    position: absolute;
    top: -146px;
    right: -335.6px;
  }

  .container {
    margin: 0px 165px;
  }

  .cards {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: 1fr 1fr;
    gap: 56px 30px;
    margin-bottom: 260px;
  }

  .logo {
    width: 111px;
    height: 28px;
  }
  
  /* .linear-gradient-bg {
    background: linear-gradient(var(--white), #F0F1FF);
    padding: 0px 165px;
  } */
  .single-card {
    padding: 64px 32px 138px;
    background: linear-gradient(var(--orange), var(--pink-gradient));
    border-radius: 15px;
    margin-top: 24px;
  }

  p {
    margin-bottom: 40px;
    margin-top: 29px;
  }

  /* .check-out {
    font-weight: 500;
  } */
</style>