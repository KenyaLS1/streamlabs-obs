<template>
<div class="studio-controls row expanded">
  <scene-selector class="studio-controls-panel small-4 columns" />
  <source-selector class="studio-controls-panel small-4 columns" />
  <mixer class="studio-controls-panel small-4 columns" />
</div>
</template>

<script lang="ts" src="./StudioControls.vue.ts"></script>

<style lang="less" scoped>
@import "../styles/index";

.studio-controls {
  height: 240px;
  width: 100%;
  .padding-h-sides();
  margin: 0;
}
</style>

<style lang="less">
@import "../styles/index";

.studio-controls {
  position: relative;
}

.studio-controls-panel {
  display: flex;
  flex-direction: column;
  height: 100%;
  .padding-h-sides();
  position: relative;
}

.studio-controls-top {
  display: flex;
  flex-direction: row;
  align-items: center;
  .margin-bottom();
  justify-content: space-between;
  flex: 0 0 20px;
}

.studio-controls__label {
  color: var(--title);
  margin-bottom: 0;
}

.studio-controls-selector {
  background: var(--section);
  .radius();
  flex-grow: 1;
  overflow-y: auto;
}
</style>
