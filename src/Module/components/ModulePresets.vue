<template>
  <v-container class="module-outcomes">
    <div class="module-outcomes__container">
      <!-- <v-divider class="presets__divider"></v-divider> -->
      <div class="presets__section-title">General</div>
      <!-- <div class="presets__nopresets">No tweaking necessary</div> -->
      <v-expansion-panels accordion flat>
        <!-- QUESTION -->
        <v-expansion-panel>
          <v-expansion-panel-header disable-icon-rotate hide-actions>
            <v-text-field
              outlined
              dense
              hide-details
              placeholder="Name your video question"
              value="How would you execute?"
            ></v-text-field>
            <v-btn class="ml-2" color="red" dark depressed>
              <v-icon left>mdi-video</v-icon> Record
            </v-btn>
            <!-- <template>
                <v-icon color="green"> mdi-check </v-icon>
              </template> -->
            <template v-slot:actions>
              <!-- <v-btn><v-icon color="red"> mdi-circle </v-icon></v-btn> -->
              <v-icon color="green"> mdi-check </v-icon>
            </template>
          </v-expansion-panel-header>
          <v-expansion-panel-content>
            <div class="presets__question-video"></div>
            <div class="presets__record-button2">
              <v-tooltip left>
                <template v-slot:activator="{ on, attrs }">
                  <v-btn v-bind="attrs" class="presets__record-button mt-3 mb-3" icon v-on="on"
                    ><v-icon color="red"> mdi-circle </v-icon></v-btn
                  >
                </template>
                <span>Record Again</span>
              </v-tooltip>
              <v-tooltip right>
                <template v-slot:activator="{ on, attrs }">
                  <v-btn v-bind="attrs" class="presets__record-button mt-3 mb-3" icon v-on="on"
                    ><v-icon color="red"> mdi-trash-can-outline </v-icon></v-btn
                  >
                </template>
                <span>Delete Question</span>
              </v-tooltip>
            </div>
          </v-expansion-panel-content>
        </v-expansion-panel>
        <!-- QUESTION -->
        <v-expansion-panel>
          <v-expansion-panel-header disable-icon-rotate hide-actions>
            <v-text-field
              outlined
              dense
              hide-details
              placeholder="Name your video question"
              value="What was the most difficult thing you had to do in life?"
            ></v-text-field>
            <v-btn class="ml-2" color="red" dark depressed>
              <v-icon left>mdi-video</v-icon> Record
            </v-btn>
            <!-- <template>
                <v-icon color="green"> mdi-check </v-icon>
              </template> -->
            <template v-slot:actions>
              <!-- <v-btn><v-icon color="red"> mdi-circle </v-icon></v-btn> -->
              <v-icon color="green"> mdi-check </v-icon>
            </template>
          </v-expansion-panel-header>
          <v-expansion-panel-content>
            <div class="presets__question-video"></div>
            <div class="presets__record-button2">
              <v-tooltip left>
                <template v-slot:activator="{ on, attrs }">
                  <v-btn v-bind="attrs" class="presets__record-button mt-3 mb-3" icon v-on="on"
                    ><v-icon color="red"> mdi-circle </v-icon></v-btn
                  >
                </template>
                <span>Record Again</span>
              </v-tooltip>
              <v-tooltip right>
                <template v-slot:activator="{ on, attrs }">
                  <v-btn v-bind="attrs" class="presets__record-button mt-3 mb-3" icon v-on="on"
                    ><v-icon color="red"> mdi-trash-can-outline </v-icon></v-btn
                  >
                </template>
                <span>Delete Question</span>
              </v-tooltip>
            </div>
          </v-expansion-panel-content>
        </v-expansion-panel>
        <!-- QUESTION -->
        <v-expansion-panel>
          <v-expansion-panel-header disable-icon-rotate hide-actions>
            <v-text-field
              outlined
              dense
              hide-details
              placeholder="Name your video question"
              value="What was your 'ah ha' moment?"
            ></v-text-field>
            <v-btn class="ml-2" color="red" dark depressed>
              <v-icon left>mdi-video</v-icon> Record
            </v-btn>
            <!-- <template>
                <v-icon color="green"> mdi-check </v-icon>
              </template> -->
            <template v-slot:actions>
              <!-- <v-btn><v-icon color="red"> mdi-circle </v-icon></v-btn> -->
              <v-icon color="green"> mdi-check </v-icon>
            </template>
          </v-expansion-panel-header>
          <v-expansion-panel-content>
            <div class="presets__question-video"></div>
            <div class="presets__record-button2">
              <v-tooltip left>
                <template v-slot:activator="{ on, attrs }">
                  <v-btn v-bind="attrs" class="presets__record-button mt-3 mb-3" icon v-on="on"
                    ><v-icon color="red"> mdi-circle </v-icon></v-btn
                  >
                </template>
                <span>Record Again</span>
              </v-tooltip>
              <v-tooltip right>
                <template v-slot:activator="{ on, attrs }">
                  <v-btn v-bind="attrs" class="presets__record-button mt-3 mb-3" icon v-on="on"
                    ><v-icon color="red"> mdi-trash-can-outline </v-icon></v-btn
                  >
                </template>
                <span>Delete Question</span>
              </v-tooltip>
            </div>
          </v-expansion-panel-content>
        </v-expansion-panel>

        <!-- QUESTION -->
        <v-expansion-panel>
          <v-expansion-panel-header disable-icon-rotate hide-actions>
            <v-text-field
              outlined
              dense
              hide-details
              placeholder="Name your video question"
              value="What problem would it be?"
            ></v-text-field>
            <v-btn class="ml-2" color="red" dark depressed>
              <v-icon left>mdi-video</v-icon> Record
            </v-btn>
            <!-- <template>
                <v-icon color="green"> mdi-check </v-icon>
              </template> -->
            <template v-slot:actions>
              <!-- <v-btn><v-icon color="red"> mdi-circle </v-icon></v-btn> -->
              <v-icon color="green"> mdi-check </v-icon>
            </template>
          </v-expansion-panel-header>
          <v-expansion-panel-content>
            <div class="presets__question-video"></div>
            <div class="presets__record-button2">
              <v-tooltip left>
                <template v-slot:activator="{ on, attrs }">
                  <v-btn v-bind="attrs" class="presets__record-button mt-3 mb-3" icon v-on="on"
                    ><v-icon color="red"> mdi-circle </v-icon></v-btn
                  >
                </template>
                <span>Record Again</span>
              </v-tooltip>
              <v-tooltip right>
                <template v-slot:activator="{ on, attrs }">
                  <v-btn v-bind="attrs" class="presets__record-button mt-3 mb-3" icon v-on="on"
                    ><v-icon color="red"> mdi-trash-can-outline </v-icon></v-btn
                  >
                </template>
                <span>Delete Question</span>
              </v-tooltip>
            </div>
          </v-expansion-panel-content>
        </v-expansion-panel>
        <!-- QUESTION -->
        <v-expansion-panel>
          <v-expansion-panel-header disable-icon-rotate hide-actions>
            <v-text-field
              outlined
              dense
              hide-details
              placeholder="Name your video question"
              value="If you had a Wikipedia page, what would it say?"
            ></v-text-field>
            <v-btn class="ml-2" color="red" dark depressed>
              <v-icon left>mdi-video</v-icon> Record
            </v-btn>
            <!-- <template>
                <v-icon color="green"> mdi-check </v-icon>
              </template> -->
            <template v-slot:actions>
              <!-- <v-btn><v-icon color="red"> mdi-circle </v-icon></v-btn> -->
              <v-icon color="green"> mdi-check </v-icon>
            </template>
          </v-expansion-panel-header>
          <v-expansion-panel-content>
            <div class="presets__question-video"></div>
            <div class="presets__record-button2">
              <v-tooltip left>
                <template v-slot:activator="{ on, attrs }">
                  <v-btn v-bind="attrs" class="presets__record-button mt-3 mb-3" icon v-on="on"
                    ><v-icon color="red"> mdi-circle </v-icon></v-btn
                  >
                </template>
                <span>Record Again</span>
              </v-tooltip>
              <v-tooltip right>
                <template v-slot:activator="{ on, attrs }">
                  <v-btn v-bind="attrs" class="presets__record-button mt-3 mb-3" icon v-on="on"
                    ><v-icon color="red"> mdi-trash-can-outline </v-icon></v-btn
                  >
                </template>
                <span>Delete Question</span>
              </v-tooltip>
            </div>
          </v-expansion-panel-content>
        </v-expansion-panel>
        <!-- QUESTION -->
        <v-expansion-panel>
          <v-expansion-panel-header disable-icon-rotate hide-actions>
            <v-text-field
              outlined
              dense
              hide-details
              placeholder="Name your video question"
              value=""
            ></v-text-field>
            <v-btn class="ml-2" color="red" dark depressed>
              <v-icon left>mdi-video</v-icon> Record
            </v-btn>
            <!-- <template>
                <v-icon color="green"> mdi-check </v-icon>
              </template> -->
            <template v-slot:actions>
              <!-- <v-btn><v-icon color="red"> mdi-circle </v-icon></v-btn> -->
              <v-icon color="green"> mdi-check </v-icon>
            </template>
          </v-expansion-panel-header>
          <v-expansion-panel-content>
            <div class="presets__question-video"></div>
            <div class="presets__record-button2">
              <v-tooltip left>
                <template v-slot:activator="{ on, attrs }">
                  <v-btn v-bind="attrs" class="presets__record-button mt-3 mb-3" icon v-on="on"
                    ><v-icon color="red"> mdi-circle </v-icon></v-btn
                  >
                </template>
                <span>Record Again</span>
              </v-tooltip>
              <v-tooltip right>
                <template v-slot:activator="{ on, attrs }">
                  <v-btn v-bind="attrs" class="presets__record-button mt-3 mb-3" icon v-on="on"
                    ><v-icon color="red"> mdi-trash-can-outline </v-icon></v-btn
                  >
                </template>
                <span>Delete Question</span>
              </v-tooltip>
            </div>
          </v-expansion-panel-content>
        </v-expansion-panel>
      </v-expansion-panels>
      <div class="presets__add-video mt-3">
        <v-icon color="grey lighten-1" large>mdi-plus</v-icon>
      </div>
      <v-divider class="presets__divider"></v-divider>
      <div class="presets__section-title">Instructions</div>
      <Instruct v-model="setupInstructions" />
      <v-divider class="presets__divider"></v-divider>
      <div class="presets__section-title">Defaults</div>

      <v-select :items="group" label="What activity group does this belong to?" outlined></v-select>
      <v-select
        :items="required"
        label="Is this activity required for participants to complete?"
        outlined
      ></v-select>

      <!-- <v-select
        :items="lockOrder"
        label="Lock activity group and placement order?"
        outlined
      ></v-select> -->
      <v-select :items="deliverable" label="Is this a deliverable?" outlined></v-select>
      <!-- <v-select
        :items="accessibility"
        label="Make this activity accessible to participants anytime?"
        outlined
      ></v-select> -->
      <v-select
        :items="endEarly"
        label="Allow participants to end program early after completion of this activity?"
        outlined
      ></v-select>
      <!-- POST-ACTIVITY REFLECTION -->
      <!-- <v-text-field
        label="Post-Activity Reflection"
        placeholder="Now that you know the scope of the project, provide a summary of your interpretation."
        outlined
        hide-details
      ></v-text-field>
      <div class="presets__reflection">
        <v-btn class="presets__reflection-buttons" small depressed outlined>Save</v-btn>
        <v-btn class="presets__reflection-buttons" small depressed outlined>Preview</v-btn>
      </div> -->
      <v-divider class="presets__divider"></v-divider>
      <!-- If activity is required, show button below, make tooltip show up while disabled, right now tooltip doesn't show up -->
      <!-- <div>
        <v-tooltip bottom>
          <template v-slot:activator="{ on, attrs }">
            <v-btn color="red" disabled v-bind="attrs" v-on="on">Delete Activity</v-btn>
          </template>
          <span>Required activities cannot be deleted</span>
        </v-tooltip>
      </div> -->
      <!-- Delete break when the two delete buttons above and below have been integrated as one solution -->
      <br />
      <!-- If activity is optional, show button below -->
      <div><v-btn color="red" dark depressed>Delete Activity</v-btn></div>
    </div>
  </v-container>
</template>

<script lang="ts">
import { defineComponent } from '@vue/composition-api';
import Instruct from './ModuleInstruct.vue';
import { group, required, deliverable, endEarly, maxMinutes } from './const';
// import gql from 'graphql-tag';

export default defineComponent({
  name: 'ModulePresets',
  components: {
    Instruct
  },
  data() {
    return {
      maxMinutes,
      group,
      required,
      deliverable,
      endEarly,
      minutes: '3',
      groupActivity: 'Project',
      requiredActivity: 'Yes',
      deliverableActivity: 'Yes',
      endEarlyActivity: 'Creator has not allowed participants to end early after this activity',
      setupInstructions: {
        description: '',
        instructions: ['', '', '']
      }
    };
  }
  // setup() {
  //   const presets = reactive({
  //     group: ['Setup', 'Project', 'Screening', 'Internship'],
  //     required: ['Creator requires this activity', 'Yes', 'No'],
  //     lockOrder: ['Creator locked activity group and placement order', 'Yes', 'No'],
  //     deliverable: ['Yes', 'No'],
  //     notifications: ['Creator turned on by default', 'Turn on', 'Turn off'],
  //     accessibility: [
  //       'Creator has turned off accessibility anytime',
  //       'Creator has turned on accessibility anytime',
  //       'Yes',
  //       'No'
  //     ],
  //     endEarly: [
  //       'Creator has not allowed participants to end early after this activity',
  //       'Creator has allow end early option only at preset order placement',
  //       'Yes',
  //       'No'
  //     ]
  //   });
  //   const setupInstructions = ref({
  //     description: '',
  //     instructions: ['', '', '']
  //   });
  //   return {
  //     ...toRefs(presets),
  //     setupInstructions
  //   };
  // }
});
</script>

<style lang="scss">
.v-btn:not(.v-btn--round).v-size--default {
  max-width: fit-content;
  // width: fit-content;
}
.v-expansion-panel-header {
  // padding: 0px !important;
}
.presets {
  &__add-video {
    border-radius: 5px;
    border: 1px dashed #dedede;
    width: 92%;
    margin: auto;
    text-align: center;
  }
  &__record-button2 {
    // justify-content: center;
    // align-items: center;
    text-align: center;
    margin-top: auto;
  }

  &__record-button {
    // justify-content: center;
    // align-items: center;
    // text-align: center;
  }

  &__question-video {
    background-color: #dedede;
    height: 300px;
    // text-align: center;
    margin: 16px 24px;
  }

  &__reflection-buttons {
    margin-right: 10px;
    margin-top: 10px;
  }

  &__reflection {
    margin-left: auto;
  }

  &__divider {
    margin-top: 40px;
    margin-bottom: 40px;
  }

  &__section-title {
    color: #000000;
    font-size: 25px;
    font-weight: 800;
    text-align: center;
    margin-bottom: 40px;
  }

  &__nopresets {
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
}
</style>
