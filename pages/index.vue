<template>
  <div @click="generate()">
    <card :field="field" :trend="trend"/>
  </div>
</template>



<script>
import card from "~/components/card.vue";
export default {
  components: {
    card
  },
  data() {
    return {
      field: "Tap the card to",
      trend: "Begin",
      trends: [
        { field: "Technology", trend: "Blockchain" },
        { field: "Technology", trend: "Behavioural Revolution" },
        { field: "Technology", trend: "Diagnosis" },
        { field: "Technology", trend: "Materials" },
        { field: "Technology", trend: "Edutainment" },
        { field: "Technology", trend: "Apps 2.0" },

        { field: "Market", trend: "Reputation Trading" },
        {
          field: "Market",
          trend: "Co-creation & Collaboration"
        },
        { field: "Market", trend: "Cross Industry Business Model" },
        { field: "Market", trend: "Bitcoin" },
        { field: "Market", trend: "Freesumerism" },

        { field: "Environment", trend: "Green conscience diffusion" },
        { field: "Environment", trend: "Smart service generations" },
        { field: "Environment", trend: "Mobility Revolution" },
        { field: "Environment", trend: "Sustainable Industry and Retail" },
        { field: "Environment", trend: "Biomimicry" },

        { field: "Population", trend: "Falling Fertility" },
        { field: "Population", trend: "Bio Printing" },
        { field: "Population", trend: "Elderly life enhancement" },
        { field: "Population", trend: "Human memory enhancement" },
        { field: "Population", trend: "DNA based diets" },

        { field: "Society", trend: "Localism" },
        { field: "Society", trend: "Gender ambiguity" },
        { field: "Society", trend: "Rising Inequality" },
        { field: "Society", trend: "Welfare State Reductions" },
        { field: "Society", trend: "Mass unemployment by AI" },

        { field: "Culture", trend: "Data Visualisation Diffusion" },
        { field: "Culture", trend: "Spiritual and Holistic Lifestyle" },
        { field: "Culture", trend: "Bio-organic and slow food culture" },
        { field: "Culture", trend: "Tech Detox" },
        { field: "Culture", trend: "Lifelong learning" }
      ]
    };
  },
  methods: {
    generate: function() {
      let i = parseInt(Math.random() * 31);
      console.log(i);
      this.field = this.trends[i].field;
      this.trend = this.trends[i].trend;
    }
  }
};
</script>