<template>
  <div class="card">
    <div class="card-header text-white bg-primary">{{ mission }} : 1233445</div>
    <div class="card-body">
      <!-- <h5 class="card-title">Special title treatment</h5>
        <p class="card-text">
          With supporting text below as a natural lead-in to additional content.
        </p>
        <a href="#" class="btn btn-primary">Go somewhere</a> -->
      <table class="table table-bordered table-hover shadow-lg">
        <thead>
          <tr class="table-info">
            <th>
              <!-- <div class="row">
          <div class="col-md-6">-->
              Prod No.
              <!-- </div> -->
              <!-- </div> -->
            </th>
            <th scope="col">
              <!-- <div class="row"> -->
              <!-- <div class="col-md-6"> -->
              Name
              <!-- </div> -->
              <!-- </div> -->
            </th>
            <th scope="col">Description</th>
            <th scope="col">Qty</th>
            <th scope="col">Price</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>15909</td>
            <td>Jyoti Jadhav</td>
            <td>{{ mission }}: {{ task }}{{ actionType }} - {{ action }}</td>
            <td>
              <input
                type="text"
                class="form-control"
                placeholder="Enter Qty"
                v-model="qty1"
                id="inputDefault"
              />
            </td>
            <td>&euro; {{ qty1 * 150 }}</td>
          </tr>
          <tr v-for="(item,index) in rowData" :key="index">
            <td>15909</td>
            <td>Jyoti Jadhav</td>
            <td>
              {{ item.mission }}: {{ item.task }}{{ item.actionType }} -
              {{ item.action }}
            </td>
            <td>
              <input
                type="text"
                class="form-control"
                placeholder="Enter Qty"
                v-model="rowData[index].qty"
                id="index"
              />
            </td>
            <td>&euro; {{ rowData[index].qty * 150 }}</td>
          </tr>
        </tbody>
      </table>
      <button
        type="button"
        class="btn btn-primary float-right"
        @click="addItem"
      >
        <span><i class="fas fa-plus-circle"></i></span>
      </button>
    </div>
  </div>
</template>
<script>
export default {
  props: ["Qty", "mission", "task", "actionType", "action"],
  data() {
    return {
      qty1: this.Qty,
      rowData: [],
    };
  },
  methods: {
    addItem() {
      var my_object = {
        qty: this.Qty,
        mission: this.mission,
        task: this.task,
        action: this.action,
        actionType: this.actionType,
      };
      this.rowData.push(my_object);
      console.log(this.rowData);
    },
  },
};
</script>
