<template>
  <v-container class="module-default pa-0">
    <div class="module-default__instructions">
      <v-expansion-panels v-model="showInstructions" class="module-default__instructions" flat>
        <v-expansion-panel>
          <v-expansion-panel-header
            v-show="showInstructions"
            hide-actions
            class="pa-0"
            @click="showInstructions = true"
          >
            <template v-slot="{ open }">
              <v-scroll-y-transition hide-on-leave>
                <div v-if="!open" class="d-flex flex-column justify-center">
                  <v-icon color="grey lighten-2" class="d-flex justify-center">
                    mdi-chevron-down
                  </v-icon>
                  <div color="grey lighten-2" class="module-default__collapse-title">
                    INSTRUCTIONS
                  </div>
                </div>
              </v-scroll-y-transition>
            </template>
          </v-expansion-panel-header>
          <v-expansion-panel-content>
            <Instruct readonly />
            <div @click="showInstructions = true">
              <div class="module-default__collapse-title">CLOSE</div>
              <!-- <div class="hr"/> OPTIONAL -->
              <v-icon color="grey lighten-2" class="d-flex justify-center"> mdi-chevron-up </v-icon>
            </div>
          </v-expansion-panel-content>
        </v-expansion-panel>
      </v-expansion-panels>
    </div>

    <v-progress-linear
      class="module-default__collapse-divider"
      color="#dedede"
      height="2"
      value="100"
      buffer-value="100"
      stream
    />
    <!-- ENTER CONTENT HERE -->
    <!-- DESIGN YOUR ACTIVITY HERE / COMMENT OUT WHEN YOU'VE STARTED DESIGNING -->
    <!-- <div class="module-default__none">Design your activity here</div> -->
    <!-- <v-btn x-large outlined depressed>Schedule Interview Now</v-btn> -->
    <!-- <v-btn x-large outlined depressed>Start Interview</v-btn> -->
    <v-expansion-panels accordion flat>
      <v-expansion-panel class="module-default__playlist-panel">
        <v-expansion-panel-header disable-icon-rotate class="module-default__video-title">
          How would you execute?
          <!-- <template>
                <v-icon color="green"> mdi-check </v-icon>
              </template> -->
          <template v-slot:actions>
            <!-- <v-btn><v-icon color="red"> mdi-circle </v-icon></v-btn> -->
            <v-icon color="green"> mdi-check-bold </v-icon>
          </template>
        </v-expansion-panel-header>
        <v-expansion-panel-content>
          <div class="module-default__question-video d-flex justify-center">
            <v-icon x-large color="white">mdi-play</v-icon>
          </div>
          <v-tooltip right>
            <template v-slot:activator="{ on, attrs }">
              <v-btn v-bind="attrs" class="mt-3 mb-3" icon v-on="on"
                ><v-icon x-large color="red"> mdi-circle </v-icon></v-btn
              >
            </template>
            <span>Record Answer</span>
          </v-tooltip>
        </v-expansion-panel-content>
      </v-expansion-panel>
      <v-expansion-panel class="module-default__playlist-panel">
        <v-expansion-panel-header class="module-default__video-title" disable-icon-rotate>
          What was the most difficult thing you had to do in life?
          <!-- <template>
                <v-icon color="green"> mdi-check </v-icon>
              </template> -->
          <template v-slot:actions>
            <!-- <v-btn><v-icon color="red"> mdi-circle </v-icon></v-btn> -->

            <v-icon color="green"> mdi-check-bold </v-icon>
          </template>
        </v-expansion-panel-header>
        <v-expansion-panel-content>
          <div class="module-default__question-video d-flex justify-center">
            <v-icon x-large color="white">mdi-play</v-icon>
          </div>
          <v-tooltip right>
            <template v-slot:activator="{ on, attrs }">
              <v-btn v-bind="attrs" class="mt-3 mb-3" icon v-on="on"
                ><v-icon x-large color="red"> mdi-circle </v-icon></v-btn
              >
            </template>
            <span>Record Answer</span>
          </v-tooltip>
        </v-expansion-panel-content>
      </v-expansion-panel>
      <v-expansion-panel class="module-default__playlist-panel">
        <v-expansion-panel-header class="module-default__video-title" disable-icon-rotate>
          What was your 'ah ha' moment?<template v-slot:actions>
            <v-icon color="yellow"> mdi-video </v-icon>
          </template>
        </v-expansion-panel-header>
        <v-expansion-panel-content>
          <div class="module-default__question-video d-flex justify-center">
            <v-icon x-large color="white">mdi-play</v-icon>
          </div>
          <v-tooltip right>
            <template v-slot:activator="{ on, attrs }">
              <v-btn v-bind="attrs" class="mt-3 mb-3" icon v-on="on"
                ><v-icon x-large color="red"> mdi-circle </v-icon></v-btn
              >
            </template>
            <span>Record Answer</span>
          </v-tooltip>
        </v-expansion-panel-content>
      </v-expansion-panel>
      <v-expansion-panel class="module-default__playlist-panel" disabled>
        <v-expansion-panel-header class="module-default__video-title" disable-icon-rotate>
          What problem would it be?<template v-slot:actions>
            <v-icon color="yellow"> mdi-video </v-icon>
          </template>
        </v-expansion-panel-header>
        <v-expansion-panel-content>
          <div class="module-default__question-video d-flex justify-center">
            <v-icon x-large color="white">mdi-play</v-icon>
          </div>
          <v-tooltip right>
            <template v-slot:activator="{ on, attrs }">
              <v-btn v-bind="attrs" class="mt-3 mb-3" icon v-on="on"
                ><v-icon x-large color="red"> mdi-circle </v-icon></v-btn
              >
            </template>
            <span>Record Answer</span>
          </v-tooltip>
        </v-expansion-panel-content>
      </v-expansion-panel>
      <v-expansion-panel class="module-default__playlist-panel" disabled>
        <v-expansion-panel-header class="module-default__video-title" disable-icon-rotate>
          If you had a Wikipedia page, what would it say?<template v-slot:actions>
            <v-icon color="yellow"> mdi-video </v-icon>
          </template>
        </v-expansion-panel-header>
        <v-expansion-panel-content>
          <div class="module-default__question-video d-flex justify-center">
            <v-icon x-large color="white">mdi-play</v-icon>
          </div>
          <v-tooltip right>
            <template v-slot:activator="{ on, attrs }">
              <v-btn v-bind="attrs" class="mt-3 mb-3" icon v-on="on"
                ><v-icon x-large color="red"> mdi-circle </v-icon></v-btn
              >
            </template>
            <span>Record Answer</span>
          </v-tooltip>
        </v-expansion-panel-content>
      </v-expansion-panel>
    </v-expansion-panels>
    <v-btn class="mt-10" disabled x-large outlined depressed>Finish Interview</v-btn>
  </v-container>
</template>

<script lang="ts">
import { ref } from '@vue/composition-api';
import Instruct from './ModuleInstruct.vue';

export default {
  name: 'ModuleDefault',
  components: {
    Instruct
  },
  apollo: {},
  data() {
    const setupInstructions = ref({
      description: '',
      instructions: ['', '', '']
    });
    const showInstructions = ref(true);
    return {
      setupInstructions,
      showInstructions
    };
  }
};
</script>

<style lang="scss">
.v-expansion-panel-content__wrap {
  padding: 0px !important;
}
.module-default {
  &__playlist-panel {
    border-bottom: 1px solid #dedede;
  }
  &__video-title {
    font-weight: 800;
    line-height: 25px !important;
    font-size: 16px !important;
    color: #404142;
  }

  &__question-video {
    background-color: #dedede;
    height: 300px;
  }
  &__none {
    border-radius: 5px;
    // border: 1px solid #dedede;
    height: 100px;
    text-align: center;
    background-color: #dedede;
    font-weight: 700;
    color: #ffffff;
    font-size: 18px;
    padding-top: 35px;
  }

  &__collapse-divider {
    margin-top: 15px;
    // margin-bottom: 75px;
    margin-right: none;
    margin-left: none;
    padding-right: none;
    padding-left: none;
    width: 100%;
  }

  &__collapse-title {
    color: #dedede;
    text-align: center;
    text-transform: uppercase;
    font-weight: 900;
    letter-spacing: 1px;
    font-size: 13px;
    //  text-uppercase font-weight-bold text-subtitle-2 text-center
  }

  &__container {
    width: 100%;
    // padding: none;
    // margin: none;
    margin-top: 0px;
    padding: 0px;
  }
  &__employer-title {
    font-size: 25px;
    font-weight: 700;
  }

  &__scope {
    font-size: 22px;
    font-weight: 800;
    text-align: center;
    max-width: 95%;
    margin: auto;
  }
  &__youtube {
    height: 400px;
    width: 95%;
    border-radius: 25px;
    // margin: 0px;
    background-color: #dedede;

    // text-align: center;
    // justify-content: center;
    // align-items: center;
    // padding-top: auto;
    // padding-bottom: auto;
  }
  &__about {
    font-size: 15px;
    font-weight: 700;
    text-align: center;
    max-width: 90%;
    margin: auto;
    line-height: 30px;
  }

  &__faq {
    font-size: 15px;
    font-weight: 700;
    text-align: center;
    max-width: 90%;
    margin: auto;
    line-height: 30px;
  }

  &__faq-chat {
    display: flex;
    flex-direction: column;
    text-align: left;
    margin-bottom: 5%;
  }
  &__faq-chat-line {
    margin: 5px;
  }

  &__faq-avatar {
    margin: 5px;
  }

  &__faq-question {
    // text-align: left;
    font-family: 'Raleway';
    font-size: 16px;
    font-weight: 800;
    color: #404142;
  }

  &__faq-answer {
    text-align: left;
    font-family: 'Raleway';
    font-size: 13px;
    font-weight: 500;
    letter-spacing: 0px;
    color: white;
    font-style: italic;
  }

  &__faq-answer-dark {
    text-align: left;
    font-family: 'Raleway';
    font-size: 13px;
    font-weight: 500;
    letter-spacing: 0px;
    color: #404142;
    font-style: italic;
  }

  &__faq-answer-dark-highlight {
    text-align: left;
    font-family: 'Raleway';
    font-size: 13px;
    font-weight: 800;
    letter-spacing: 0px;
    color: #404142;
  }

  &__specs-title {
    font-weight: 800;
  }
}
</style>
