<script setup lang="ts"></script>
<template>
  <div class="Container">
    <div class="Results">
      <div class="Left">
        <h2 class="Light-lavender">Your Result</h2>
        <div class="Circle">
          <div style="font-size: 56px; line-height: 60px">76</div>
          <div class="Light-lavender" style="opacity: 50%">of 100</div>
        </div>
        <h1>Great</h1>
        <p class="Light-lavender">
          You scored higher than 65% of the people who have taken these tests.
        </p>
      </div>
      <div class="Right">
        <h2>Summary</h2>
        <div
          class="Card"
          style="background-color: var(--Light-red-background); color: var(--Light-red)"
        >
          <div>
            <img src="@/assets/result-summary/icon-reaction.svg" alt="icon-reaction" />
            <div>Reaction</div>
          </div>
          <div style="color: var(--Light-lavender); font-weight: 700">
            <div style="color: var(--Dark-gray-blue); font-weight: 700">80</div>
            / 100
          </div>
        </div>
        <div
          class="Card"
          style="background-color: var(--Orangey-yellow-background); color: var(--Orangey-yellow)"
        >
          <div>
            <img src="@/assets/result-summary/icon-memory.svg" alt="icon-memory" />
            <div>Memory</div>
          </div>
          <div style="color: var(--Light-lavender); font-weight: 700">
            <div style="color: var(--Dark-gray-blue); font-weight: 700">92</div>
            / 100
          </div>
        </div>
        <div
          class="Card"
          style="background-color: var(--Green-teal-background); color: var(--Green-teal)"
        >
          <div>
            <img src="@/assets/result-summary/icon-verbal.svg" alt="icon-verbal" />
            <div>Verbal</div>
          </div>
          <div style="color: var(--Light-lavender); font-weight: 700">
            <div style="color: var(--Dark-gray-blue); font-weight: 700">61</div>
            / 100
          </div>
        </div>
        <div
          class="Card"
          style="background-color: var(--Cobalt-blue-background); color: var(--Cobalt-blue)"
        >
          <div>
            <img src="@/assets/result-summary/icon-visual.svg" alt="icon-visual" />
            <div>Visual</div>
          </div>
          <div style="color: var(--Light-lavender); font-weight: 700">
            <div style="color: var(--Dark-gray-blue); font-weight: 700">72</div>
            / 100
          </div>
        </div>
        <button>
          <!-- <p> -->
          Continue
          <!-- </p> -->
        </button>
      </div>
    </div>

    <div class="attribution">
      Challenge by
      <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>.
      Coded by <a href="#">Natchanonnn</a>.
    </div>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=DM+Sans&family=Hanken+Grotesk:wght@500;700;800&display=swap');
.Container {
  /* ### Primary */
  --Light-red: hsl(0, 100%, 67%);
  --Orangey-yellow: hsl(39, 100%, 56%);
  --Green-teal: hsl(166, 100%, 37%);
  --Cobalt-blue: hsl(234, 85%, 45%);
  --Light-red-background: hsla(0, 100%, 67%, 10%);
  --Orangey-yellow-background: hsl(39, 100%, 56%, 10%);
  --Green-teal-background: hsl(166, 100%, 37%, 10%);
  --Cobalt-blue-background: hsl(234, 85%, 45%, 10%);

  /* Gradients */
  --Light-slate-blue: hsl(252, 100%, 67%); /*(background)*/
  --Light-royal-blue: hsl(241, 81%, 54%); /*(background)*/
  --Violet-blue: hsla(256, 72%, 46%, 1); /*(circle)*/
  --Persian-blue: hsla(241, 72%, 46%, 0); /*(circle)*/

  /* Neutral */
  --White: hsl(0, 0%, 100%);
  --Pale-blue: hsl(221, 100%, 96%);
  --Light-lavender: hsl(241, 100%, 89%);
  --Dark-gray-blue: hsl(224, 30%, 27%);
  --border-radius: 20px;

  /* Fonts */
  font-family: 'Hanken Grotesk';
  /* Weights: 500, 700, 800 */
  display: flex;
  justify-content: center;
  text-align: center;
  font-size: 16px;
}
.Pale-blue {
  color: var(--Pale-blue);
}
.Light-lavender {
  color: var(--Light-lavender);
}
.Results {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 720px;
  height: 480px;
  border-radius: var(--border-radius);
  box-shadow: rgba(136, 165, 191, 0.48) 6px 2px 16px 0px,
    rgba(255, 255, 255, 0.8) -6px -2px 16px 0px;
  background: var(--White);
}
p {
  font-size: 18px;
}
.Left {
  background: linear-gradient(0deg, var(--Light-royal-blue), var(--Light-slate-blue));
  border-radius: var(--border-radius);
  height: 400px;
  color: var(--White);
  width: 50%;
  height: 100%;
  padding: 20px 20px 30px 20px;
  display: flex;
  justify-content: space-around;
  flex-direction: column;
  align-items: center;
}
.Right {
  height: 100%;
  width: 50%;
  color: blackl;
  display: flex;
  flex-direction: column;
  text-align: left;
  padding: 20px 40px 20px 40px;
}
h1 {
  font-weight: 800;
}
.Circle {
  border-radius: 50%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 150px;
  height: 150px;
  margin: 20px;
  background: linear-gradient(0deg, var(--Persian-blue), var(--Violet-blue));
}
.Card {
  border-radius: 8px;
  height: 48px;
  margin: 10px 0 10px 0;
  display: flex;
  justify-content: space-between;
  align-content: center;
}
.Card > div {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0 10px;
}
.Card > div > div {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 8px;
}
button {
  height: 48px;
  border-radius: 24px;
  background-color: var(--Dark-gray-blue);
  color: var(--White);
  font-size: 16px;
  outline: none;
  border: none;
  margin: 28px 0;
}
button:active {
  background: linear-gradient(0deg, var(--Light-royal-blue), var(--Light-slate-blue));
}
h2 {
  font-weight: 800;
  margin-bottom: 24px;
}
p {
  width: 230px;
  opacity: 80%;
}
@media (max-width: 1024px) {
  .Container {
    flex-direction: column;
    min-height: 100vh;
  }
  .Results {
    flex-direction: column;
    margin: 0;
    height: 100%;
    width: 100%;
  }
  .Left {
    height: 100vw;
    width: 100%;
    margin: 0;
    padding: 0;
    justify-content: center;
    border-radius: 0  0  var(--border-radius) var(--border-radius);
  }
  .Right {
    height: 50%;
    width: 100%;
    padding: 20px;  
  }
  p {
    width: 300px;
  }
  .Circle {
    margin: 0;
  }
}
</style>
