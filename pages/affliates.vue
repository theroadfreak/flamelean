<template>
  <section class="container my-4">
    <div v-for="item in listOfItems" class="py-5">
      <h3>{{ item.title }}</h3>
      <h4>Subject Lines:</h4>
      <ol style="list-style: lower-alpha">
        <li v-for="line in item.subjectLines">{{ line }}</li>
      </ol>
      <p v-for="p in item.paragraphs" v-html="p"></p>
      <img
        v-if="item.picture"
        :src="require(`@/assets/images/` + item.picture)"
        :width="item.width"
        alt="picture"
        class="object-fit-contain"
      />
      <p v-for="p in item.restOfParagraphs" v-html="p"></p>
    </div>
  </section>
</template>

<script>
export default {
  name: "affliates",
  data() {
    return {
      listOfItems: [
        {
          title: "Email Swipe 1 - Science Mech Tease",
          subjectLines: [
            "Do THIS to burn fat in the morning",
            "Jessica lost 40 lbs in 2 months WITHOUT surgery",
            "Harvard: diabetics should try THIS for weight loss",
          ],
          paragraphs: [
            "Harvard Medical School is proving a macronutrient has dramatic effects on diabetics…",
            "Improving insulin sensitivity and helping you feel fuller for longer.",
            "In fact, Jessica tried it and lost 40 lbs of weight in 2 just months!",
            "Not only was she forced to buy a whole new wardrobe…",
            "But Jessica finally felt in control of her blood sugar levels…",
            "The natural way and with zero stress.",
            "<span class='text-primary text-decoration-underline'> >> Try THIS Harvard-approved macronutrient today</span>>",
          ],
        },
        {
          title: "Email Swipe 2 - Celebrity Gossip",
          subjectLines: [
            "Kim Kardadshian before and after (pics inside)",
            "Kim Kardashian’s dieting secret",
            "REVEALED: Kim Kardashian weight loss truth",
          ],
          paragraphs: [
            "I just read a post on Kim Kardashian…",
            "About how she really lost 16 pounds in 3 weeks.",
            "Take a look:",
          ],
          picture:
            "tsl/the-biggest-suspect-section/kim-kardashian-transformation.png",
          width: 500,
          restOfParagraphs: [
            "Rumors are circulating Hollywood right now…",
            "That Kim and other A-List celebrities (Rebel Wilson, Elon Musk and more)...",
            "Are using a diabetes medication to slim down effortlessly.",
            "Here’s the thing…",
            "The medication they’re injecting themselves with costs an eye watering $1,300 per month.",
            "Plus, it comes with a boxed warning…",
            "The strongest safety-related warning required by the FDA!",
            "The good news is…",
            "There’s a more natural, safer, cheaper alternative to this medication.",
            "It works the same way by:",
            "Using that sugar for energy instead of storing it as stubborn fat…",
            "Decreasing your appetite and helping you lose weight effortlessly",
            "So, if you have trouble losing weight and managing your blood sugar levels…",
            "The easiest thing you can do is…",
            "=> Try THIS natural, safe, affordable alternative every morning",
            "It’s going to give your body everything it needs to start burning fat again…",
            "And manage your blood glucose without the stress.",
            "Stay healthy!",
          ],
        },
        {
          title: "Email Swipe 3 - Shorter Celeb Gossip",
          subjectLines: [
            "lose 40 pounds in 2 months like Kim Kardashian",
            "Try Kim Kardashian’s weight loss 'secret'",
            "lose weight FASTER than Kim Kardashian (safely)",
          ],
          paragraphs: [
            "Have you noticed celebrities getting skinnier than ever before",
          ],
          picture: "affliate/affliate1.png",
          width: 300,
          restOfParagraphs: [
            "It’s got nothing to do with a new workout routine, diet, or surgery procedure.",
            "It’s a lot more simple than that.",
            "You see, it’s been rumored the Kardashian’s are taking diabetes medication…",
            "That comes at an eye-watering price.",
            "$1,300 fee per month to be exact.",
            "And it’s not for the faint-hearted.",
            "It has to be injected once weekly in either the thigh, stomach, or upper arm.",
            "Luckily, there’s a more natural, cheaper, invasion-free alternative.",
            "Jessica tried it and lost 40 pounds in just 2 months.",
            "I was shocked when I saw her drop from 210 to 170 pounds!",
            "I practically begged for her secret.",
            "And she generously revealed everything you need to know, here…",
            "<span class='text-primary text-decoration-underline'> => lose 40 pounds in 2 months like Kim Kardashian </span>",
            "<span class='text-primary text-decoration-underline'> => Try Kim Kardashian’s weight loss “secret” </span>",
            "<span class='text-primary text-decoration-underline'> => lose weight FASTER than Kim Kardashian (safely) </span>",
          ],
        },
        {
          title: "Email Swipe 4 - Problem / Solution",
          subjectLines: [
            "THIS is why you can’t lose weight",
            "TRUTH about diabetes and weight loss",
            "losing weight is easy once you know THIS",
            "Rebel Wilson before and after (pics inside)",
          ],
          paragraphs: [
            "It’s got nothing to do with a new workout routine, diet, or surgery procedure.",
            "Want to know why you find it so hard to lose weight?",
            "Well, if you have diabetes there’s a very simple reason that not many people talk about.",
            "You see, my friend Jessica has suffered from Type 2 diabetes for over 9 years.",
            "She piled on 40 pounds in the space of 6 months…",
            "And was struggling to lose it ever since.",
            "So, when she saw A-List celebs like Kim Kardashian, Elon Musk, and Rebel Wilson suddenly drop weight in the blink of an eye…",
            "She demanded to know their secret.",
          ],
          picture: "affliate/affliate1.png",
          width: 300,
          restOfParagraphs: [
            "Not only did she discover some of them were taking a diabetes medication (and forcing it to sellout nationwide)...",
            "But she uncovered exactly WHY it works so well at helping you lose weight.",
            "Regardless of whether you’re obese, have diabetes, or are perfectly healthy.",
            "You see, it has everything to do with a hormone inside of you that…",
            "When switched “off” can cause you to always feel hungry…",
            "Crave sweet and sugary foods…",
            "And hold onto fat for dear life.",
            "Making it near impossible to shift.",
            "But the beauty of this hormone is that, once it’s switched “on”…",
            "The reverse happens.",
            "Jesscia was able to lose 40 pounds in the space of 2 months!",
            "WITHOUT injecting herself with needles, or asking for prescriptions like the celebs.",
            "<span class='text-primary text-decoration-underline'> => You can read Jessica’s full story here</span>",
            "If you’ve been trying to lose weight for a long time, or gain control of your fluctuating blood sugar levels…",
            "Then I encourage you to click the link now while her site’s still online.",
            "Big pharma is trying frantically to take it down…",
            "Because she’s sharing a more natural alternative than what they have to offer you.",
            "Stay healthy!",
          ],
        },
      ],
    };
  },
};
</script>

<style scoped></style>
