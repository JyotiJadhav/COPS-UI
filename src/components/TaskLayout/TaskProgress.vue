<template>
  <div class="row" style="margin-bottom:3%">
    <div class="col-md-12">
      <div class="progress">
        <div
          class="progress-bar bg-success"
          role="progressbar"
          style="width: 25%"
          aria-valuenow="25"
          aria-valuemin="0"
          aria-valuemax="100"
        ></div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "TaskProgress",
};
</script>