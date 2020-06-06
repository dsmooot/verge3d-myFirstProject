<template>
  <div>
    <div :id="containerId">
      <div
        id="fullscreen_button"
        class="fullscreen-button fullscreen-open"
        title="Toggle fullscreen mode"
      ></div>
    </div>
    <div id="hide_button">HIDE</div>
    <div id="show_button">SHOW</div>
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