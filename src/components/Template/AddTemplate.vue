<template>
  <form>
    <fieldset>
      <div class="row my-2">
        <div class="col-md-6">
          <h5>Mission</h5>
        </div>
        <div class="col-md-6">
          <h5>Tasks</h5>
        </div>
      </div>
      <div class="row">
        <div class="col-md-6">
          <!-- <h5>Mission</h5> -->
          <select class="form-control shadow" id="exampleSelect1">
            <option>Centiro Internet</option>
            <option>2</option>
            <option>3</option>
            <option>4</option>
            <option>5</option>
          </select>
        </div>
        <div class="col-md-6">
          <div>
            <!-- <h5>Tasks</h5> -->

            <select class="form-control shadow" id="exampleSelect1">
              <option>Sector Retail(Team & Personal)</option>
              <option>2</option>
              <option>3</option>
              <option>4</option>
              <option>5</option>
            </select>
          </div>
        </div>
      </div>
    </fieldset>
    <fieldset>
      <div class="row my-2">
        <div class="col-md-6">
          <h5>Action</h5>
        </div>
        <div class="col-md-6">
          <h5>Action Type</h5>
        </div>
      </div>
      <div class="row">
        <div class="col-md-6">
          <!-- <h5>Action</h5> -->
          <select class="form-control shadow" id="exampleSelect1">
            <option>Team Trasformers</option>
            <option>Team R&D</option>
            <option>3</option>
            <option>4</option>
            <option>5</option>
          </select>
        </div>
        <div class="col-md-6">
          <div>
            <!-- <h5>Action Type</h5> -->
            <select class="form-control shadow" id="exampleSelect1">
              <option>Internal Meeting</option>
              <option>Conference</option>
              <option>Personal Development</option>
              <option>Education</option>
            </select>
          </div>
        </div>
      </div>
    </fieldset>
    <fieldset>
      <div class="row my-2">
        <div class="col-md-6">
          <h5>Days Active</h5>
        </div>
        <div class="col-md-6">
          <h5>Time</h5>
        </div>
      </div>
      <div class="row">
        <div class="col-md-6">
          <button type="button" class="btn btn-default btn-circle">
            <div class="font-weight-bold">M</div>
          </button>
          <button type="button" class="btn btn-default btn-circle">
            <div class="font-weight-bold">T</div>
          </button>
          <button type="button" class="btn btn-default btn-circle">
            <div class="font-weight-bold">W</div>
          </button>
          <button type="button" class="btn btn-default btn-circle">
            <div class="font-weight-bold">T</div>
          </button>
          <button type="button" class="btn btn-default btn-circle">
            <div class="font-weight-bold">F</div>
          </button>
        </div>
        <div class="col-md-6 my-2">
          <input
            type="range"
            class="custom-range"
            id="customRange1"
            height="100%"
          />
        </div>
      </div>
    </fieldset>
    <div class="row my-2">
      <div class="col-md-12">
        <h5>Description</h5>
        <textarea
          class="form-control shadow"
          id="exampleTextarea"
          rows="3"
        ></textarea>
      </div>
    </div>
    <div class="row my-4">
      <div class="col-md-8">
        <select class="form-control shadow" id="exampleSelect1">
          <option>Invoiceable</option>
          <option>Non-Invoiceable</option>
          <option>Startup</option>
        </select>
      </div>
    </div>
  </form>
</template>
<style scoped>
.btn-circle {
  width: 50px;
  height: 50px;
  text-align: center;
  padding: 6px 0;
  font-size: 15px;
  line-height: 1.428571429;
  border-radius: 25px;
  border-color: black;
}
.btn:focus {
  background: #2c3e50;
  color: white;
}
</style>