<script setup lang="ts"></script>

<template>
  <section>
    <img src="/startSaving.png" />
    <div class="startSavingText">
      <h5>The Rise App</h5>
      <h2>Save for your <span class="purple">future</span></h2>
      <p>
        <span class="line-break-block">With Rise, you achieve your financial goals faster.</span>
        <span class="line-break-block">Save for school, your home, vacations, your children’s</span>
        <span class="line-break-block">future and more.</span>
      </p>
      <button>
        Start Saving
      </button>
    </div>

  </section>
</template>

<style scoped>
section {
  display: flex;
  align-items: center;
  justify-content: space-evenly;
  padding: 3rem;
}

h5,
h2 {
  font-family: Tomato Grotesk;
  font-weight: normal;
}

.startSavingText {
  display: flex;
  flex-direction: column;
  text-align: left;
}

.purple {
  color: #8C5FF7;
}

button {
  background-color: #07969E;
  color: #FFFFFF;
  padding: 16px 3rem;
  border-radius: 5px;
  border: none;
  font-weight: bold;
  font-size: 1rem;
  align-self: flex-start;
}

@media (max-width: 1024px) {
  section {
    display: none;
  }
}
</style>
