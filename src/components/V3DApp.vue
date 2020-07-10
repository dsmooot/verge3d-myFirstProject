<template>
  <div>
    <div :id="containerId">
      <div
        id="fullscreen_button"
        class="fullscreen-button fullscreen-open"
        title="Toggle fullscreen mode"
      ></div>
    </div>
    <!-- <div id="hide_button">HIDE</div> -->
    <!-- <div id="show_button">SHOW</div> -->
    <div class="left-panel-center">
      <div id="left_panel" class="left-panel">
        <div id="fold_button" class="fold-button">Fold</div>
        <div id="unfold_button" class="unfold-button">Unfold</div>
        <div id="annotation_knife_button" class="annotation-button">Info</div>
      </div>
    </div>
    <div class="right-panel-center">
      <div id="right_panel" class="right-panel">
        <div id="plastic_button" class="plastic-button">blue</div>
        <div id="carbon_button" class="carbon-button">grey</div>
        <div id="wood_button" class="wood-button">wood</div>
      </div>
    </div>
  </div>
</template>

<script>
import * as V3DApp from "../v3dApp/swiss_army_knife.js";

export default {
  name: "V3DApp",

  data: function() {
    return {
      containerId: V3DApp.CONTAINER_ID
    };
  },

  mounted: function() {
    V3DApp.createApp();
  }
};
</script>

<style>
@import "../v3dApp/swiss_army_knife.css";
</style>