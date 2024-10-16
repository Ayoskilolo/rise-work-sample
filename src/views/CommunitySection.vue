<script setup lang="ts">
</script>

<template>
  <section id="community">
    <div>
      <h2>Join The Rise Community</h2>
      <p id="normal-text">
        <span class="line-break-block">If you want to go far, go together. Our Telegram community</span>
        <span class="line-break-block"> surrounds you with others who can help you along your financial </span>
        <span class="line-break-block">financial journey with tips, support, advice and learning. It's completely</span>
        <span class="line-break-block">free and open to new and seasoned investors.</span>
      </p>
      <p id="mobile-text">If you want to go far, go together.</p>
      <button>
        Join our Community
      </button>
    </div>

    <img src="/community.png" alt="" class="communityImg">
  </section>
</template>

<style scoped>
h2 {
  font-size: 40px;
  font-family: Tomato Grotesk;
  font-weight: normal;
}

#community {
  margin-top: 3rem;
  margin-bottom: 4rem;
  display: flex;
  align-items: center;
  color: #2D2D2D;
  justify-content: space-between;
}

#mobile-text {
  display: none;
}

button {
  background-color: #A0DDE2;
  color: #2D2D2D;
  padding: 16px 3rem;
  border-radius: 5px;
  border: none;
  font-weight: bold;
  font-size: 1rem;
  align-self: flex-start;
}

@media (max-width: 1024px) {
  h2 {
    line-height: 40px;
  }

  #community {
    flex-direction: column-reverse;
    text-align: center;
  }

  #normal-text {
    display: none;
  }

  #mobile-text {
    display: block;
  }

  .communityImg {
    height: 250px;
    margin-bottom: 2rem;
  }
}
</style>
