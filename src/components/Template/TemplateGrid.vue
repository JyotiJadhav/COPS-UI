<template>
    <div class="row">
      <div class="col-md-12">
        <table class="table table-bordered table-hover shadow-lg">
          <thead>
            <tr class="table-primary">
              <th>
                <!-- <div class="row">
          <div class="col-md-6">-->
                Mission
                <!-- </div> -->
                <!-- </div> -->
              </th>
              <th scope="col">
                <!-- <div class="row"> -->
                <!-- <div class="col-md-6"> -->
                Task
                <!-- </div> -->
                <!-- </div> -->
              </th>
              <th scope="col">Action Type</th>
              <th scope="col">Action</th>
              <th scope="col">Product</th>
              <th scope="col">Comment</th>
              <th scope="col">Invoicing</th>
              <th scope="col">
                <!-- <div class="row"> -->
                <!-- <div class="col-md-12"> -->
                Monday 03 Aug
                <!-- </div> -->
                <!-- </div> -->
              </th>
              <th scope="col">
                Tuesday 04 Aug
                <!-- <div class="row">
            <div class="col-md-12">
              <h4>04 Aug</h4>
            </div>
          </div>-->
              </th>
              <th scope="col">
                <!-- <div class="row"> -->
                <!-- <div class="col-md-6"> -->
                Wednesday
                <!-- </div> -->
                <!-- </div> -->
                <!-- <div class="row"> -->
                <!-- <div class="col-md-12"> -->
                <!-- <h4> -->
                05 Aug
                <!-- </h4> -->
                <!-- </div> -->
                <!-- </div> -->
              </th>
              <th scope="col">Thursday 06 Aug</th>
              <th scope="col">Friday 07 Aug</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <!-- <td>
          <div class="row">
            <div class="col-md-8">
              <input type="range" class="custom-range" />
            </div>
            <div class="col-md-4">00.30</div>
          </div>
        </td>-->
              <td>
                <select
                  class="form-control"
                  v-model="mission"
                  id="exampleSelect1"
                >
                  <option>Centiro Internal</option>
                  <option>Abasic S.L.</option>
                  <option>BAHAG</option>
                  <option>Centiro R&D</option>
                  <option>Staples</option>
                </select>
              </td>
              <td>
                <select class="form-control" v-model="task" id="exampleSelect1">
                  <option>Carrier Integration</option>
                  <option>Project Work</option>
                </select>
              </td>
              <td>
                <select
                  class="form-control"
                  v-model="actionType"
                  id="exampleSelect1"
                >
                  <option>Internal Meeting</option>
                  <option>Requirement Defination</option>
                  <option>Project Startup</option>
                  <option>Build and Develop</option>
                  <option>Deployments</option>
                </select>
              </td>
              <td>
                <select
                  class="form-control"
                  v-model="action"
                  id="exampleSelect1"
                >
                  <option>Internal Meeting</option>
                  <option>Requirement Defination</option>
                  <option>Project Startup</option>
                  <option>Build and Develop</option>
                  <option>Deployments</option>
                </select>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>product 1</option>
                  <option>product 2</option>
                </select>
              </td>
              <td>
                <textarea
                  class="form-control"
                  id="exampleTextarea"
                  rows="1"
                ></textarea>
              </td>
              <td>
                <select
                  class="form-control"
                  v-model="selected"
                  id="exampleSelect1"
                  @change="hideTable()"
                >
                  <option>Startup</option>
                  <option>Invoiceable</option>
                  <option>Non-Invoicing</option>
                </select>
              </td>
              <td>00.30</td>
              <td>00.30</td>
              <td>00.30</td>
              <td>00.30</td>
              <td>00.30</td>
            </tr>
            <tr v-show="show">
              <!-- <td>
          <div class="row">
            <div class="col-md-8">
              <input type="range" class="custom-range" />
            </div>
            <div class="col-md-4">00.30</div>
          </div>
        </td>-->
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Centiro Internal</option>
                  <option>Abasic S.L.</option>
                  <option>BAHAG</option>
                  <option>Centiro R&D</option>
                  <option>Staples</option>
                </select>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Carrier Integration</option>
                  <option>Project Work</option>
                </select>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Internal Meeting</option>
                  <option>Requirement Defination</option>
                  <option>Project Startup</option>
                  <option>Build and Develop</option>
                  <option>Deployments</option>
                </select>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Internal Meeting</option>
                  <option>Requirement Defination</option>
                  <option>Project Startup</option>
                  <option>Build and Develop</option>
                  <option>Deployments</option>
                </select>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>product 1</option>
                  <option>product 2</option>
                </select>
              </td>
              <td>
                <textarea
                  class="form-control"
                  id="exampleTextarea"
                  rows="1"
                ></textarea>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Startup</option>
                  <option>Invoiceable</option>
                  <option>Non-Invoicing</option>
                </select>
              </td>
              <td>00.30</td>
              <td>05.00</td>
              <td>01.30</td>
              <td>00.30</td>
              <td>00.30</td>
            </tr>
            <tr v-show="show">
              <!-- <td>
          <div class="row">
            <div class="col-md-8">
              <input type="range" class="custom-range" />
            </div>
            <div class="col-md-4">00.30</div>
          </div>
        </td>-->
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Centiro Internal</option>
                  <option>Abasic S.L.</option>
                  <option>BAHAG</option>
                  <option>Centiro R&D</option>
                  <option>Staples</option>
                </select>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Carrier Integration</option>
                  <option>Project Work</option>
                </select>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Internal Meeting</option>
                  <option>Requirement Defination</option>
                  <option>Project Startup</option>
                  <option>Build and Develop</option>
                  <option>Deployments</option>
                </select>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Internal Meeting</option>
                  <option>Requirement Defination</option>
                  <option>Project Startup</option>
                  <option>Build and Develop</option>
                  <option>Deployments</option>
                </select>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>product 1</option>
                  <option>product 2</option>
                </select>
              </td>
              <td>
                <textarea
                  class="form-control"
                  id="exampleTextarea"
                  rows="1"
                ></textarea>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Startup</option>
                  <option>Invoiceable</option>
                  <option>Non-Invoicing</option>
                </select>
              </td>
              <td>00.30</td>
              <td>01.30</td>
              <td>01.30</td>
              <td>00.30</td>
              <td>00.30</td>
            </tr>
            <tr v-show="show">
              <!-- <td>
          <div class="row">
            <div class="col-md-8">
              <input type="range" class="custom-range" />
            </div>
            <div class="col-md-4">00.30</div>
          </div>
        </td>-->
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Centiro Internal</option>
                  <option>Abasic S.L.</option>
                  <option>BAHAG</option>
                  <option>Centiro R&D</option>
                  <option>Staples</option>
                </select>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Carrier Integration</option>
                  <option>Project Work</option>
                </select>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Internal Meeting</option>
                  <option>Requirement Defination</option>
                  <option>Project Startup</option>
                  <option>Build and Develop</option>
                  <option>Deployments</option>
                </select>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Internal Meeting</option>
                  <option>Requirement Defination</option>
                  <option>Project Startup</option>
                  <option>Build and Develop</option>
                  <option>Deployments</option>
                </select>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>product 1</option>
                  <option>product 2</option>
                </select>
              </td>
              <td>
                <textarea
                  class="form-control"
                  id="exampleTextarea"
                  rows="1"
                ></textarea>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Startup</option>
                  <option>Invoiceable</option>
                  <option>Non-Invoicing</option>
                </select>
              </td>
              <td>02.30</td>
              <td>01.00</td>
              <td>01.30</td>
              <td>00.30</td>
              <td>00.30</td>
            </tr>
            <tr v-show="show">
              <!-- <td>
          <div class="row">
            <div class="col-md-8">
              <input type="range" class="custom-range" />
            </div>
            <div class="col-md-4">00.30</div>
          </div>
        </td>-->
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Centiro Internal</option>
                  <option>Abasic S.L.</option>
                  <option>BAHAG</option>
                  <option>Centiro R&D</option>
                  <option>Staples</option>
                </select>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Carrier Integration</option>
                  <option>Project Work</option>
                </select>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Internal Meeting</option>
                  <option>Requirement Defination</option>
                  <option>Project Startup</option>
                  <option>Build and Develop</option>
                  <option>Deployments</option>
                </select>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Internal Meeting</option>
                  <option>Requirement Defination</option>
                  <option>Project Startup</option>
                  <option>Build and Develop</option>
                  <option>Deployments</option>
                </select>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>product 1</option>
                  <option>product 2</option>
                </select>
              </td>
              <td>
                <textarea
                  class="form-control"
                  id="exampleTextarea"
                  rows="1"
                ></textarea>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Startup</option>
                  <option>Invoiceable</option>
                  <option>Non-Invoicing</option>
                </select>
              </td>
              <td>02.30</td>
              <td>----</td>
              <td>01.30</td>
              <td>01.30</td>
              <td>03.30</td>
            </tr>
            <tr v-show="show">
              <!-- <td>
          <div class="row">
            <div class="col-md-8">
              <input type="range" class="custom-range" />
            </div>
            <div class="col-md-4">00.30</div>
          </div>
        </td>-->
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Centiro Internal</option>
                  <option>Abasic S.L.</option>
                  <option>BAHAG</option>
                  <option>Centiro R&D</option>
                  <option>Staples</option>
                </select>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Carrier Integration</option>
                  <option>Project Work</option>
                </select>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Internal Meeting</option>
                  <option>Requirement Defination</option>
                  <option>Project Startup</option>
                  <option>Build and Develop</option>
                  <option>Deployments</option>
                </select>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Internal Meeting</option>
                  <option>Requirement Defination</option>
                  <option>Project Startup</option>
                  <option>Build and Develop</option>
                  <option>Deployments</option>
                </select>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>product 1</option>
                  <option>product 2</option>
                </select>
              </td>
              <td>
                <textarea
                  class="form-control"
                  id="exampleTextarea"
                  rows="1"
                ></textarea>
              </td>
              <td>
                <select class="form-control" id="exampleSelect1">
                  <option>Startup</option>
                  <option>Invoiceable</option>
                  <option>Non-Invoicing</option>
                </select>
              </td>
              <td>01.30</td>
              <td>----</td>
              <td>01.30</td>
              <td>04.30</td>
              <td>02.30</td>
            </tr>
            <tr class="table-dark" v-show="show">
              <!-- <td>
          <div class="row">
            <div class="col-md-8">
              <input type="range" class="custom-range" />
            </div>
            <div class="col-md-4">00.30</div>
          </div>
        </td>-->
              <td colspan="7">Total</td>

              <td>08.00</td>
              <td>08.00</td>
              <td>08.00</td>
              <td>08.00</td>
              <td>08.00</td>
            </tr>
          </tbody>
        </table>
        <InvoiceGrid
          v-show="showInvice"
          :mission="mission"
          :task="task"
          :action="action"
          :actionType="actiontype"
          :Qty="Qty"
        ></InvoiceGrid>
      </div>
    </div>
</template>
<script>
import InvoiceGrid from "../Invoice/InvoiceGrid.vue";

export default {
  components: { InvoiceGrid },

  name: "Weekly",
  data() {
    return {
      show: true,
      showInvice: false,
      selected: "Startup",
      mission: "Centiro Internal",
      task: "Carrier Integration",
      actionType: "Internal Meeting",
      action: "Requirement Defination",
      Qty: 1,
    };
  },
  methods: {
    hideTable() {
      if (this.selected === "Invoiceable") {
        this.show = false;
        this.showInvice = true;
      } else {
        this.show = true;
        this.showInvice = false;
      }
    },
  },
};
</script>