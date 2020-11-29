<template>
  <div>
    <div class="row"></div>

    <div class="row">
      <div class="col-md-4 my-4">
        <h3>
          Total:
          <small class="text-muted">40:00:00</small>
        </h3>
      </div>
      <!-- <div class="col-md-3 my-4">
      <div style="float: right">
        <button type="button" class="btn btn-primary">
          <span><i class="fas fa-plus-circle"></i> Create New Template</span>
        </button>
      </div>
 </div> -->
      <div class="col-md-4 my-4">
        <select class="form-control" id="exampleSelect1">
          <option>Template 1</option>
          <option>Template 2</option>
        </select>
      </div>
      <div class="col-md-4 my-4">
        <div style="float: right">
          <button type="button" class="btn btn-primary">
            <span><i class="fas fa-plus-circle"></i></span>
          </button>
        </div>
        <!-- <div
        class="btn-group btn-group-toggle"
        style="float: right"
        data-toggle="buttons"
      >
        <label class="btn btn-primary">
          <input type="radio" name="options" id="Calender" autocomplete="off" />
          <i class="fas fa-calendar-alt"></i>
        </label>
        <label class="btn btn-primary active">
          <input type="radio" name="options" id="Daily" autocomplete="off" v-model="checked" /> Daily
        </label> -->
        <!-- <label class="btn btn-primary">
          <input type="radio" name="options" id="Weekly" autocomplete="off" />
          Weekly
        </label> -->
        <!-- </div>  -->
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "TaskLayout",
};
</script>

