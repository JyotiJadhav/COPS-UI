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
        <select
          class="form-control"
          id="exampleSelect1"
          v-if="viewType == 'Weekly'"
        >
          <option>Template 1</option>
          <option>Template 2</option>
        </select>
      </div>
      <div class="col-md-4 my-4">
        <div style="float: right" v-if="viewType == 'Weekly'">
          <button type="button" class="btn btn-primary" @click="openModal">
            <span><i class="fas fa-plus-circle"></i></span>
          </button>
          <AddTempateModal ref="modal"></AddTempateModal>
        </div>
        <div
          class="btn-group btn-group-toggle"
          style="float: right"
          data-toggle="buttons"
        >
          <label class="btn btn-primary">
            <input
              type="radio"
              name="options"
              id="Calender"
              autocomplete="off"
            />
            <i class="fas fa-calendar-alt"></i>
          </label>
          <label class="btn btn-primary active">
            <input
              type="radio"
              name="options"
              id="daily"
              value="Daily"
              v-model="viewType"
              autocomplete="off"
            />
            Daily
          </label>
          <label class="btn btn-primary">
            <input
              type="radio"
              name="options"
              id="weekly"
              value="Weekly"
              v-model="viewType"
              autocomplete="off"
            />
            Weekly
          </label>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import AddTempateModal from "../Template/AddTemplateLayout";

export default {
  name: "TaskLayout",
  components: { AddTempateModal },
  methods: {
    openModal() {
      this.$refs.modal.show();
    }, //executing the show method of child
  },
  props: ["type"],
  data: function () {
    return {
      viewType: this.type,
    };
  },
};
</script>

