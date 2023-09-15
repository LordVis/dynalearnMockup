<template id="body1">
  <!--  -->
  <div class="dark-dropdown, entity1"> <!-- Sun -->
    <h3>Entity</h3>
    <select v-model="selectedOptionEntity1" id="entity1">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <h5>Related to</h5>
    <select v-model="connectedTo1_1" id="connected1">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
  </div>
  <div class="dark-dropdown, entity2"> <!-- Earth -->
    <h3>Entity</h3>
    <select v-model="selectedOptionEntity2" id="entity2">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <h5>Related to</h5>
    <select v-model="connectedTo2_1" id="connected2">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <h5>Related to</h5>
    <select v-model="connectedTo2_2" id="connected3">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <h5>Related to</h5>
    <select v-model="connectedTo2_3" id="connected4">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
  </div>
  <div class="dark-dropdown, entity3"> <!-- Atmosphere -->
    <h3>Entity</h3>
    <select v-model="selectedOptionEntity3" id="entity3">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <h5>Related to</h5>
    <select v-model="connectedTo3_1" id="connected5">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <h5>Related to</h5>
    <select v-model="connectedTo3_2" id="connected6">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <h5>Related to</h5>
    <select v-model="connectedTo3_3" id="connected7">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
  </div>
  <div class="dark-dropdown, entity4"> <!-- Ocean -->
    <h3>Entity</h3>
    <select v-model="selectedOptionEntity4" id="entity4">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <h5>Related to</h5>
    <select v-model="connectedTo4_1" id="connected8">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <h5>Related to</h5>
    <select v-model="connectedTo4_2" id="connected9">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <h5>Related to</h5>
    <select v-model="connectedTo4_3" id="connected10">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
  </div>
  <!--  -->

  <div class="dark-dropdown, Quantity1"> <!-- Sunlight -->
    <h3>Quantity</h3>
    <select v-model="selectedOptionQuantity1" id="quantity1">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <select v-model="selectedOptionQuantity1Amount">
      <option v-for="option in dropdownForQuantity" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <h5>Related to</h5>
    <select v-model="connectedTo5" id="connected11">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <select v-model="connectedToRelation5" id="relationship1">
      <option v-for="option in dropdownConnectionPositiveOrNot" :value="option.value" :key="option.value">
        {{option.label}}</option>
    </select>

  </div>
  <div class="dark-dropdown, Quantity2"> <!-- Surface temperature -->
    <h3>Quantity</h3>
    <select v-model="selectedOptionQuantity2" id="quantity2">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <select v-model="selectedOptionQuantity2Amount">
      <option v-for="option in dropdownForQuantity" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <h5>Related to</h5>
    <select v-model="connectedTo6" id="connected12">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <select v-model="connectedToRelation6" id="relationship2">
      <option v-for="option in dropdownConnectionPositiveOrNot" :value="option.value" :key="option.value">
        {{option.label}}</option>
    </select>
  </div>
  <div class="dark-dropdown, Quantity3"> <!-- Radiated heat -->
    <h3>Quantity</h3>
    <select v-model="selectedOptionQuantity3" id="quantity3">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <select v-model="selectedOptionQuantity3Amount">
      <option v-for="option in dropdownForQuantity" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <h5>Related to</h5>
    <select v-model="connectedTo7" id="connected13">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <select v-model="connectedToRelation7" id="relationship3">
      <option v-for="option in dropdownConnectionPositiveOrNot" :value="option.value" :key="option.value">
        {{option.label}}</option>
    </select>
  </div>
  <div class="dark-dropdown, Quantity4"> <!-- Bio Diversity -->
    <h3>Quantity</h3>
    <select v-model="selectedOptionQuantity4" id="quantity4">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <select v-model="selectedOptionQuantity4Amount">
      <option v-for="option in dropdownForQuantity" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
  </div>
  <div class="dark-dropdown, Quantity5"> <!-- reflected heat radiation -->
    <h3>Quantity</h3>
    <select v-model="selectedOptionQuantity5" id="quantity5">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <select v-model="selectedOptionQuantity5Amount">
      <option v-for="option in dropdownForQuantity" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <h5>Related to</h5>
    <select v-model="connectedTo8" id="connected14">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <select v-model="connectedToRelation8" id="relationship4">
      <option v-for="option in dropdownConnectionPositiveOrNot" :value="option.value" :key="option.value">
        {{option.label}}</option>
    </select>
  </div>
  <div class="dark-dropdown, Quantity6"> <!-- greenhouse gas -->
    <h3>Quantity</h3>
    <select v-model="selectedOptionQuantity6" id="quantity6">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <select v-model="selectedOptionQuantity6Amount">
      <option v-for="option in dropdownForQuantity" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <h5>Related to</h5>
    <select v-model="connectedTo9_1" id="connected15">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <select v-model="connectedToRelation9_1" id="relationship5">
      <option v-for="option in dropdownConnectionPositiveOrNot" :value="option.value" :key="option.value">
        {{option.label}}</option>
    </select>
    <h5>Related to</h5>
    <select v-model="connectedTo9_2" id="connected16">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <select v-model="connectedToRelation9_2" id="relationship6">
      <option v-for="option in dropdownConnectionPositiveOrNot" :value="option.value" :key="option.value">
        {{option.label}}</option>
    </select>
  </div>
  <div class="dark-dropdown, Quantity7"> <!-- Tempature -->
    <h3>Quantity</h3>
    <select v-model="selectedOptionQuantity7" id="quantity7">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <select v-model="selectedOptionQuantity7Amount">
      <option v-for="option in dropdownForQuantity" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <h5>Related to</h5>
    <select v-model="connectedTo10_1" id="connected17">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <select v-model="connectedToRelation10_1" id="relationship7">
      <option v-for="option in dropdownConnectionPositiveOrNot" :value="option.value" :key="option.value">
        {{option.label}}</option>
    </select>
    <h5>Related to</h5>
    <select v-model="connectedTo10_2" id="connected18">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <select v-model="connectedToRelation10_2" id="relationship8">
      <option v-for="option in dropdownConnectionPositiveOrNot" :value="option.value" :key="option.value">
        {{option.label}}</option>
    </select>
  </div>
  <div class="dark-dropdown, Quantity8"> <!-- Tempature -->
    <h3>Quantity</h3>
    <select v-model="selectedOptionQuantity8" id="quantity8">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <select v-model="selectedOptionQuantity8Amount">
      <option v-for="option in dropdownForQuantity" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <h5>Related to</h5>
    <select v-model="connectedTo11" id="connected19">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <select v-model="connectedToRelation11" id="relationship9">
      <option v-for="option in dropdownConnectionPositiveOrNot" :value="option.value" :key="option.value">
        {{option.label}}</option>
    </select>
  </div>
  <div class="dark-dropdown, Quantity9"> <!-- biodiversity -->
    <h3>Quantity</h3>
    <select v-model="selectedOptionQuantity9" id="quantity9">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <select v-model="selectedOptionQuantity9Amount">
      <option v-for="option in dropdownForQuantity" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
  </div>
  <div class="dark-dropdown, Quantity10"> <!-- Acidity -->
    <h3>Quantity</h3>
    <select v-model="selectedOptionQuantity10" id="quantity10">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <select v-model="selectedOptionQuantity10Amount">
      <option v-for="option in dropdownForQuantity" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <h5>Related to</h5>
    <select v-model="connectedTo12" id="connected20">
      <option v-for="option in dropdownOptions" :value="option.value" :key="option.value">{{option.label}}</option>
    </select>
    <select v-model="connectedToRelation12" id="relationship10">
      <option v-for="option in dropdownConnectionPositiveOrNot" :value="option.value" :key="option.value">
        {{option.label}}</option>
    </select>
  </div>
  <div class="buttons">
    <a class="btn btn-white btn-mid button1" @click="checkGame">Check</a>
    <a class="btn btn-white btn-mid button2" @click="runGame">Run</a>
  </div>
</template>

<script>
  export default {
    created() {
      // this.selectedOptionEntity1 = this.dropdownOptions[0].value;
      // this.selectedOptionEntity2 = this.dropdownOptions[0].value;
      // this.selectedOptionEntity3 = this.dropdownOptions[0].value;
      // this.selectedOptionEntity4 = this.dropdownOptions[0].value;

      // this.selectedOptionQuantity1 = this.dropdownOptions[0].value;
      // this.selectedOptionQuantity2 = this.dropdownOptions[0].value;
      // this.selectedOptionQuantity3 = this.dropdownOptions[0].value;
      // this.selectedOptionQuantity4 = this.dropdownOptions[0].value;
      // this.selectedOptionQuantity5 = this.dropdownOptions[0].value;
      // this.selectedOptionQuantity6 = this.dropdownOptions[0].value;
      // this.selectedOptionQuantity7 = this.dropdownOptions[0].value;
      // this.selectedOptionQuantity8 = this.dropdownOptions[0].value;
      // this.selectedOptionQuantity9 = this.dropdownOptions[0].value;
      // this.selectedOptionQuantity10 = this.dropdownOptions[0].value;

      // this.connectedTo1_1 = this.dropdownOptions[0].value;
      // this.connectedTo2_1 = this.dropdownOptions[0].value;
      // this.connectedTo2_2 = this.dropdownOptions[0].value;
      // this.connectedTo2_3 = this.dropdownOptions[0].value;
      // this.connectedTo3_1 = this.dropdownOptions[0].value;
      // this.connectedTo3_2 = this.dropdownOptions[0].value;
      // this.connectedTo3_3 = this.dropdownOptions[0].value;
      // this.connectedTo4_1 = this.dropdownOptions[0].value;
      // this.connectedTo4_2 = this.dropdownOptions[0].value;
      // this.connectedTo4_3 = this.dropdownOptions[0].value;

      // this.connectedTo5 = this.dropdownOptions[0].value;
      // this.connectedToRelation5 = this.dropdownConnectionPositiveOrNot[0].value;
      // this.connectedTo6 = this.dropdownOptions[0].value;
      // this.connectedToRelation6 = this.dropdownConnectionPositiveOrNot[0].value;
      // this.connectedTo7 = this.dropdownOptions[0].value;
      // this.connectedToRelation7 = this.dropdownConnectionPositiveOrNot[0].value;
      // this.connectedTo8 = this.dropdownOptions[0].value;
      // this.connectedToRelation8 = this.dropdownConnectionPositiveOrNot[0].value;
      // this.connectedTo9_1 = this.dropdownOptions[0].value
      // this.connectedToRelation9_1 = this.dropdownConnectionPositiveOrNot[0].value
      // this.connectedTo9_2 = this.dropdownOptions[0].value
      // this.connectedToRelation9_2 = this.dropdownConnectionPositiveOrNot[0].value
      // this.connectedTo10_1 = this.dropdownOptions[0].value
      // this.connectedToRelation10_1 = this.dropdownConnectionPositiveOrNot[0].value
      // this.connectedTo10_2 = this.dropdownOptions[0].value
      // this.connectedToRelation10_2 = this.dropdownConnectionPositiveOrNot[0].value
      // this.connectedTo11 = this.dropdownOptions[0].value
      // this.connectedToRelation11 = this.dropdownConnectionPositiveOrNot[0].value
      // this.connectedTo12 = this.dropdownOptions[0].value
      // this.connectedToRelation12 = this.dropdownConnectionPositiveOrNot[0].value

      this.selectedOptionQuantity1Amount = this.dropdownForQuantity[1].value
      this.selectedOptionQuantity2Amount = this.dropdownForQuantity[1].value
      this.selectedOptionQuantity3Amount = this.dropdownForQuantity[1].value
      this.selectedOptionQuantity4Amount = this.dropdownForQuantity[1].value
      this.selectedOptionQuantity5Amount = this.dropdownForQuantity[1].value
      this.selectedOptionQuantity6Amount = this.dropdownForQuantity[1].value
      this.selectedOptionQuantity7Amount = this.dropdownForQuantity[1].value
      this.selectedOptionQuantity8Amount = this.dropdownForQuantity[1].value
      this.selectedOptionQuantity9Amount = this.dropdownForQuantity[1].value
      this.selectedOptionQuantity10Amount = this.dropdownForQuantity[1].value



      this.selectedOptionEntity1 = this.dropdownOptions[9].value;
      this.selectedOptionEntity2 = this.dropdownOptions[4].value;
      this.selectedOptionEntity3 = this.dropdownOptions[2].value;
      this.selectedOptionEntity4 = this.dropdownOptions[6].value;

      this.selectedOptionQuantity1 = this.dropdownOptions[10].value;
      this.selectedOptionQuantity2 = this.dropdownOptions[11].value;
      this.selectedOptionQuantity3 = this.dropdownOptions[7].value;
      this.selectedOptionQuantity4 = this.dropdownOptions[3].value;
      this.selectedOptionQuantity5 = this.dropdownOptions[8].value;
      this.selectedOptionQuantity6 = this.dropdownOptions[5].value;
      this.selectedOptionQuantity7 = this.dropdownOptions[12].value;
      this.selectedOptionQuantity8 = this.dropdownOptions[12].value;
      this.selectedOptionQuantity9 = this.dropdownOptions[3].value;
      this.selectedOptionQuantity10 = this.dropdownOptions[1].value;

      this.connectedTo1_1 = this.dropdownOptions[10].value;
      this.connectedTo2_1 = this.dropdownOptions[11].value;
      this.connectedTo2_2 = this.dropdownOptions[7].value;
      this.connectedTo2_3 = this.dropdownOptions[3].value;
      this.connectedTo3_1 = this.dropdownOptions[5].value;
      this.connectedTo3_2 = this.dropdownOptions[8].value;
      this.connectedTo3_3 = this.dropdownOptions[12].value;
      this.connectedTo4_1 = this.dropdownOptions[12].value;
      this.connectedTo4_2 = this.dropdownOptions[3].value;
      this.connectedTo4_3 = this.dropdownOptions[1].value;

      this.connectedTo5 = this.dropdownOptions[11].value;
      this.connectedToRelation5 = this.dropdownConnectionPositiveOrNot[1].value;
      this.connectedTo6 = this.dropdownOptions[7].value;
      this.connectedToRelation6 = this.dropdownConnectionPositiveOrNot[1].value;
      this.connectedTo7 = this.dropdownOptions[8].value;
      this.connectedToRelation7 = this.dropdownConnectionPositiveOrNot[1].value;
      this.connectedTo8 = this.dropdownOptions[12].value;
      this.connectedToRelation8 = this.dropdownConnectionPositiveOrNot[1].value;
      this.connectedTo9_1 = this.dropdownOptions[8].value
      this.connectedToRelation9_1 = this.dropdownConnectionPositiveOrNot[1].value
      this.connectedTo9_2 = this.dropdownOptions[1].value
      this.connectedToRelation9_2 = this.dropdownConnectionPositiveOrNot[1].value
      this.connectedTo10_1 = this.dropdownOptions[12].value
      this.connectedToRelation10_1 = this.dropdownConnectionPositiveOrNot[1].value
      this.connectedTo10_2 = this.dropdownOptions[3].value
      this.connectedToRelation10_2 = this.dropdownConnectionPositiveOrNot[2].value
      this.connectedTo11 = this.dropdownOptions[3].value
      this.connectedToRelation11 = this.dropdownConnectionPositiveOrNot[2].value
      this.connectedTo12 = this.dropdownOptions[3].value
      this.connectedToRelation12 = this.dropdownConnectionPositiveOrNot[2].value
    },
    name: 'App',
    methods: {
      checkGame() {
        document.getElementById("entity1").style.color = 'white';
        document.getElementById("entity2").style.color = 'white';
        document.getElementById("entity3").style.color = 'white';
        document.getElementById("entity4").style.color = 'white';
        document.getElementById("quantity1").style.color = 'white';
        document.getElementById("quantity2").style.color = 'white';
        document.getElementById("quantity3").style.color = 'white';
        document.getElementById("quantity4").style.color = 'white';
        document.getElementById("quantity5").style.color = 'white';
        document.getElementById("quantity6").style.color = 'white';
        document.getElementById("quantity7").style.color = 'white';
        document.getElementById("quantity8").style.color = 'white';
        document.getElementById("quantity9").style.color = 'white';
        document.getElementById("quantity10").style.color = 'white';
        document.getElementById("connected1").style.color = 'white';
        document.getElementById("connected2").style.color = 'white';
        document.getElementById("connected3").style.color = 'white';
        document.getElementById("connected4").style.color = 'white';
        document.getElementById("connected5").style.color = 'white';
        document.getElementById("connected6").style.color = 'white';
        document.getElementById("connected7").style.color = 'white';
        document.getElementById("connected8").style.color = 'white';
        document.getElementById("connected9").style.color = 'white';
        document.getElementById("connected10").style.color = 'white';
        document.getElementById("connected11").style.color = 'white';
        document.getElementById("connected12").style.color = 'white';
        document.getElementById("connected13").style.color = 'white';
        document.getElementById("connected14").style.color = 'white';
        document.getElementById("connected15").style.color = 'white';
        document.getElementById("connected16").style.color = 'white';
        document.getElementById("connected17").style.color = 'white';
        document.getElementById("connected18").style.color = 'white';
        document.getElementById("connected19").style.color = 'white';
        document.getElementById("connected20").style.color = 'white';
        document.getElementById("relationship1").style.color = 'white';
        document.getElementById("relationship2").style.color = 'white';
        document.getElementById("relationship3").style.color = 'white';
        document.getElementById("relationship4").style.color = 'white';
        document.getElementById("relationship5").style.color = 'white';
        document.getElementById("relationship6").style.color = 'white';
        document.getElementById("relationship7").style.color = 'white';
        document.getElementById("relationship8").style.color = 'white';
        document.getElementById("relationship9").style.color = 'white';
        document.getElementById("relationship10").style.color = 'white';

        if (this.selectedOptionEntity1 != this.dropdownOptions[9].value) {
          document.getElementById("entity1").style.color = 'red';
        } if (this.selectedOptionEntity2 != this.dropdownOptions[4].value) {
          document.getElementById("entity2").style.color = 'red';
        } if (this.selectedOptionEntity3 != this.dropdownOptions[2].value) {
          document.getElementById("entity3").style.color = 'red';
        } if (this.selectedOptionEntity4 != this.dropdownOptions[6].value) {
          document.getElementById("entity4").style.color = 'red';
        } if (this.selectedOptionQuantity1 != this.dropdownOptions[10].value) {
          document.getElementById("quantity1").style.color = 'red';
        } if (this.selectedOptionQuantity2 != this.dropdownOptions[11].value) {
          document.getElementById("quantity2").style.color = 'red';
        } if (this.selectedOptionQuantity3 != this.dropdownOptions[7].value) {
          document.getElementById("quantity3").style.color = 'red';
        } if (this.selectedOptionQuantity4 != this.dropdownOptions[3].value) {
          document.getElementById("quantity4").style.color = 'red';
        } if (this.selectedOptionQuantity5 != this.dropdownOptions[8].value) {
          document.getElementById("quantity5").style.color = 'red';
        } if (this.selectedOptionQuantity6 != this.dropdownOptions[5].value) {
          document.getElementById("quantity6").style.color = 'red';
        } if (this.selectedOptionQuantity7 != this.dropdownOptions[12].value) {
          document.getElementById("quantity7").style.color = 'red';
        } if (this.selectedOptionQuantity8 != this.dropdownOptions[12].value) {
          document.getElementById("quantity8").style.color = 'red';
        } if (this.selectedOptionQuantity9 != this.dropdownOptions[3].value) {
          document.getElementById("quantity9").style.color = 'red';
        } if (this.selectedOptionQuantity10 != this.dropdownOptions[1].value) {
          document.getElementById("quantity10").style.color = 'red';
        }

        if (this.connectedTo1_1 != this.dropdownOptions[10].value) {
          document.getElementById("connected1").style.color = 'red';
        } if (this.connectedTo2_1 != this.dropdownOptions[11].value) {
          document.getElementById("connected2").style.color = 'red';
        } if (this.connectedTo2_2 != this.dropdownOptions[7].value) {
          document.getElementById("connected3").style.color = 'red';
        } if (this.connectedTo2_3 != this.dropdownOptions[3].value) {
          document.getElementById("connected4").style.color = 'red';
        } if (this.connectedTo3_1 != this.dropdownOptions[5].value) {
          document.getElementById("connected5").style.color = 'red';
        } if (this.connectedTo3_2 != this.dropdownOptions[8].value) {
          document.getElementById("connected6").style.color = 'red';
        } if (this.connectedTo3_3 != this.dropdownOptions[12].value) {
          document.getElementById("connected7").style.color = 'red';
        } if (this.connectedTo4_1 != this.dropdownOptions[12].value) {
          document.getElementById("connected8").style.color = 'red';
        } if (this.connectedTo4_2 != this.dropdownOptions[3].value) {
          document.getElementById("connected9").style.color = 'red';
        } if (this.connectedTo4_3 != this.dropdownOptions[1].value) {
          document.getElementById("connected10").style.color = 'red';
        }

        if (this.connectedTo5 != this.dropdownOptions[11].value) {
          document.getElementById("connected11").style.color = 'red';
        } if (this.connectedToRelation5 != this.dropdownConnectionPositiveOrNot[1].value) {
          document.getElementById("relationship1").style.color = 'red';
        } if (this.connectedTo6 != this.dropdownOptions[7].value) {
          document.getElementById("connected12").style.color = 'red';
        } if (this.connectedToRelation6 != this.dropdownConnectionPositiveOrNot[1].value) {
          document.getElementById("relationship2").style.color = 'red';
        } if (this.connectedTo7 != this.dropdownOptions[8].value) {
          document.getElementById("connected13").style.color = 'red';
        } if (this.connectedToRelation7 != this.dropdownConnectionPositiveOrNot[1].value) {
          document.getElementById("relationship3").style.color = 'red';
        } if (this.connectedTo8 != this.dropdownOptions[12].value) {
          document.getElementById("connected14").style.color = 'red';
        } if (this.connectedToRelation8 != this.dropdownConnectionPositiveOrNot[1].value) {
          document.getElementById("relationship4").style.color = 'red';
        }

        if (this.connectedTo9_1 != this.dropdownOptions[8].value) {
          document.getElementById("connected15").style.color = 'red';
        } if (this.connectedToRelation9_1 != this.dropdownConnectionPositiveOrNot[1].value) {
          document.getElementById("relationship5").style.color = 'red';
        } if (this.connectedTo9_2 != this.dropdownOptions[1].value) {
          document.getElementById("connected16").style.color = 'red';
        } if (this.connectedToRelation9_2 != this.dropdownConnectionPositiveOrNot[1].value) {
          document.getElementById("relationship6").style.color = 'red';
        } if (this.connectedTo10_1 != this.dropdownOptions[12].value) {
          document.getElementById("connected17").style.color = 'red';
        } if (this.connectedToRelation10_1 != this.dropdownConnectionPositiveOrNot[1].value) {
          document.getElementById("relationship7").style.color = 'red';
        } if (this.connectedTo10_2 != this.dropdownOptions[3].value) {
          document.getElementById("connected18").style.color = 'red';
        } if (this.connectedToRelation10_2 != this.dropdownConnectionPositiveOrNot[2].value) {
          document.getElementById("relationship8").style.color = 'red';
        } if (this.connectedTo11 != this.dropdownOptions[3].value) {
          document.getElementById("connected19").style.color = 'red';
        } if (this.connectedToRelation11 != this.dropdownConnectionPositiveOrNot[2].value) {
          document.getElementById("relationship9").style.color = 'red';
        } if (this.connectedTo12 != this.dropdownOptions[3].value) {
          document.getElementById("connected20").style.color = 'red';
        } if (this.connectedToRelation12 != this.dropdownConnectionPositiveOrNot[2].value) {
          document.getElementById("relationship10").style.color = 'red';
        }
      },
      runGame() {
        if (this.selectedOptionQuantity1Amount == this.dropdownForQuantity[0].value && this.selectedOptionQuantity6Amount == this.dropdownForQuantity[0].value) {
          this.selectedOptionQuantity2Amount = this.dropdownForQuantity[0].value;
          this.selectedOptionQuantity3Amount = this.dropdownForQuantity[0].value;
          this.selectedOptionQuantity5Amount = this.dropdownForQuantity[0].value;
          this.selectedOptionQuantity7Amount = this.dropdownForQuantity[0].value;
          this.selectedOptionQuantity4Amount = this.dropdownForQuantity[2].value;
          this.selectedOptionQuantity8Amount = this.dropdownForQuantity[0].value;
          this.selectedOptionQuantity9Amount = this.dropdownForQuantity[2].value;
          this.selectedOptionQuantity10Amount = this.dropdownForQuantity[0].value;
        } else if (this.selectedOptionQuantity6Amount == this.dropdownForQuantity[0].value) {
          this.selectedOptionQuantity10Amount = this.dropdownForQuantity[0].value;
        } else if (this.selectedOptionQuantity5Amount == this.dropdownForQuantity[0].value) {
          this.selectedOptionQuantity7Amount = this.dropdownForQuantity[0].value;
          this.selectedOptionQuantity8Amount = this.dropdownForQuantity[0].value;
          this.selectedOptionQuantity4Amount = this.dropdownForQuantity[2].value;
        }

        if (this.selectedOptionQuantity1Amount == this.dropdownForQuantity[2].value && this.selectedOptionQuantity6Amount == this.dropdownForQuantity[2].value) {
          this.selectedOptionQuantity2Amount = this.dropdownForQuantity[2].value;
          this.selectedOptionQuantity3Amount = this.dropdownForQuantity[2].value;
          this.selectedOptionQuantity5Amount = this.dropdownForQuantity[2].value;
          this.selectedOptionQuantity7Amount = this.dropdownForQuantity[2].value;
          this.selectedOptionQuantity4Amount = this.dropdownForQuantity[0].value;
          this.selectedOptionQuantity8Amount = this.dropdownForQuantity[2].value;
          this.selectedOptionQuantity9Amount = this.dropdownForQuantity[0].value;
          this.selectedOptionQuantity10Amount = this.dropdownForQuantity[2].value;
        } else if (this.selectedOptionQuantity6Amount == this.dropdownForQuantity[2].value) {
          this.selectedOptionQuantity10Amount = this.dropdownForQuantity[2].value;
        } else if (this.selectedOptionQuantity5Amount == this.dropdownForQuantity[2].value) {
          this.selectedOptionQuantity7Amount = this.dropdownForQuantity[2].value;
          this.selectedOptionQuantity8Amount = this.dropdownForQuantity[2].value;
          this.selectedOptionQuantity4Amount = this.dropdownForQuantity[0].value;
        }
      },
    },
    data() {
      return {
        dropdownOptions: [
          { label: 'No name yet', value: 'noNameYet' }, // 0
          { label: 'Acidity', value: 'acidity' },
          { label: 'Atmosphere', value: 'atmosphere' },
          { label: 'Biodiversity', value: 'biodiversity' },
          { label: 'Earth', value: 'earth' },
          { label: 'Greenhouse gas', value: 'greenhouseGas' }, // 5
          { label: 'Ocean', value: 'ocean' },
          { label: 'Radiated heat', value: 'radiatedHeat' },
          { label: 'Reflected heat radiation', value: 'reflectedheatRadiation' },
          { label: 'Sun', value: 'sun' },
          { label: 'Sunlight', value: 'sunlight' }, // 10
          { label: 'Surface temperature', value: 'surfaceTemperature' },
          { label: 'Temperature', value: 'temperature' },
        ],
        dropdownForQuantity: [
          { label: 'Increase', value: 'increase' },
          { label: 'Stay the same', value: 'stayTheSame' },
          { label: 'Decrease', value: 'decrease' },
        ],
        dropdownConnectionPositiveOrNot: [
          { label: 'No relationship chosen', value: 'noRelationshipChosen' },
          { label: 'Positive', value: 'positive' },
          { label: 'Negative', value: 'negative' },
        ],

        selectedOptionEntity1: null,
        selectedOptionEntity2: null,
        selectedOptionEntity3: null,
        selectedOptionEntity4: null,

        selectedOptionQuantity1: null,
        selectedOptionQuantity1Amount: null, // sunlight
        selectedOptionQuantity2: null,
        selectedOptionQuantity2Amount: null, // 
        selectedOptionQuantity3: null,
        selectedOptionQuantity3Amount: null,
        selectedOptionQuantity4: null,
        selectedOptionQuantity4Amount: null,
        selectedOptionQuantity5: null,
        selectedOptionQuantity5Amount: null,
        selectedOptionQuantity6: null,
        selectedOptionQuantity6Amount: null,
        selectedOptionQuantity7: null,
        selectedOptionQuantity7Amount: null,
        selectedOptionQuantity8: null,
        selectedOptionQuantity8Amount: null,
        selectedOptionQuantity9: null,
        selectedOptionQuantity9Amount: null,
        selectedOptionQuantity10: null,
        selectedOptionQuantity10Amount: null,

        connectedTo1_1: null, // Sun

        connectedTo2_1: null, // Earth
        connectedTo2_2: null,
        connectedTo2_3: null,

        connectedTo3_1: null, // Atmosphere
        connectedTo3_2: null,
        connectedTo3_3: null,

        connectedTo4_1: null, // Ocean
        connectedTo4_2: null,
        connectedTo4_3: null,

        connectedTo5: null, // Sunlight
        connectedToRelation5: null,
        connectedTo6: null, // Surface Temp
        connectedToRelation6: null,
        connectedTo7: null, // Radiated heat
        connectedToRelation7: null,
        connectedTo8: null, // reflected heat radiation
        connectedToRelation8: null,
        connectedTo9_1: null, // greenhouse gas
        connectedToRelation9_1: null,
        connectedTo9_2: null,
        connectedToRelation9_2: null,
        connectedTo10_1: null, // Tempature
        connectedToRelation10_1: null,
        connectedTo10_2: null,
        connectedToRelation10_2: null,

        connectedTo11: null, // Tempature
        connectedToRelation11: null,
        connectedTo12: null, // Acidity
        connectedToRelation12: null,
      }
    }
  }
</script>

<style scoped>
  body {
    font: 13px/22px Helvetica;
  }

  /* Buttons */
  .button1 {
    position: absolute;
    bottom: 50px;
    left: 1020px;
  }

  .button2 {
    position: absolute;
    bottom: 50px;
    left: 900px;
  }

  .buttons {
    overflow: hidden;
  }

  .buttons>div {
    width: calc(50% - 40px);
    padding: 20px;
    float: left;
    position: fixed;
    bottom: 0;
    top: 0;
  }

  .buttons .dark {
    background: #000;
    left: 50%;
  }

  .buttons a {
    float: left;
    margin-right: 20px;
    margin-bottom: 20px;
  }

  a#link {
    position: absolute;
    left: 20px;
    bottom: 10px;
    text-decoration: none;
    color: #555;
    font-weight: bold;
  }

  .btn,
  input[type="submit"] {
    cursor: pointer;
    border-radius: 0px;
    text-decoration: none;
    padding: 12px 18px;
    font-size: 12px;
    line-height: 19px;
    text-transform: uppercase;
    font-family: 'Montserrat', sans-serif;
    font-weight: 400;
    letter-spacing: 3px;
    -webkit-transition: all .4s ease-in-out;
    -moz-transition: all .4s ease-in-out;
    -ms-transition: all .4s ease-in-out;
    -o-transition: all .4s ease-in-out;
    transition: all .4s ease-in-out;
  }

  .btn-mid {
    border-radius: 0px;
    text-decoration: none;
    padding: 14px 21px;
    font-size: 13px;
    line-height: 25px;
    text-transform: uppercase;
    font-family: 'Montserrat', sans-serif;
    font-weight: 400;
    letter-spacing: 3px;
    -webkit-transition: all .4s ease-in-out;
    -moz-transition: all .4s ease-in-out;
    -ms-transition: all .4s ease-in-out;
    -o-transition: all .4s ease-in-out;
    transition: all .4s ease-in-out;
  }

  .btn:hover,
  input[type="submit"]:hover {
    -webkit-transition: all .4s ease-in-out;
    -moz-transition: all .4s ease-in-out;
    -ms-transition: all .4s ease-in-out;
    -o-transition: all .4s ease-in-out;
    transition: all .4s ease-in-out;
  }

  .btn-white {
    border: solid 2px #fff;
    background: transparent;
    color: #fff !important;
  }

  .btn-white:hover {
    border: solid 2px #fff;
    background: #fff;
    color: #1f1f1f !important;
  }

  /* Entities, Quantites and Relations */
  .entity1 {
    /* Sun */
    color: blue;
    position: absolute;
    top: 200px;
    left: 50px;
  }

  .entity2 {
    /* Earth */
    color: blue;
    position: absolute;
    top: 300px;
    left: 400px;
  }

  .entity3 {
    /* Atmosphere */
    color: blue;
    position: absolute;
    top: 5px;
    left: 800px;
  }

  .entity4 {
    /* Ocean */
    color: blue;
    position: absolute;
    top: 100px;
    left: 1400px;
  }

  /*  */

  .Quantity1 {
    /* Sunlight */
    color: green;
    position: absolute;
    top: 500px;
    left: 10px;
  }

  .Quantity2 {
    /* Surface Temp */
    color: green;
    position: absolute;
    top: 500px;
    left: 350px;
  }

  .Quantity3 {
    /* Radiated heat */
    color: green;
    position: absolute;
    top: 600px;
    left: 700px;
  }

  .Quantity4 {
    /* Bio Diversity */
    color: green;
    position: absolute;
    top: 700px;
    left: 350px;
  }

  .Quantity5 {
    /* reflected heat radiation */
    color: green;
    position: absolute;
    top: 400px;
    left: 800px;
  }

  .Quantity6 {
    /* greenhouse gas */
    color: green;
    position: absolute;
    top: 10px;
    left: 400px;
  }

  .Quantity7 {
    /* Tempature */
    color: green;
    position: absolute;
    top: 500px;
    left: 1100px;
  }

  .Quantity8 {
    /* Tempature */
    color: green;
    position: absolute;
    top: 300px;
    left: 1200px;
  }

  .Quantity9 {
    /* biodiversity */
    color: green;
    position: absolute;
    top: 500px;
    left: 1400px;
  }

  .Quantity10 {
    /* Acidity */
    color: green;
    position: absolute;
    top: 400px;
    left: 1650px;
  }

  /*  */

  .dark-dropdown {
    background-color: #333;
    color: #fff;
    border-radius: 5px;
    padding: 15px;
  }

  select {
    background-color: #333;
    color: #fff;
    border: none;
    border-radius: 5px;
    padding: 5px;
    display: block;
  }

  option {
    background-color: #333;
    color: #fff;
  }
</style>