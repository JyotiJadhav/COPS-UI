<template>
  <div class="treeview-animated w-20 border my-4">
    <h6 class="pt-3 pl-3">Missions</h6>
    <hr />
    <ul class="treeview-animated-list mb-3">
      <li class="treeview-animated-items">
        <a class="closed">
          <i class="fas fa-angle-right"></i>
          <span>
            <i class="fas fa-users ic-w mx-1"></i>Abasic, S.L. - 1812
          </span>
        </a>
        <ul class="nested">
          <li class="treeview-animated-items">
            <a class="closed">
              <i class="fas fa-angle-right"></i>
              <span>
                <i class="fas fa-flag ic-w mx-1"></i>Carrier Integration
              </span>
            </a>
            <ul class="nested">
              <li>
                <div class="treeview-animated-element">
                  <i class="fas fa-tasks ic-w mr-1"></i>UPS US
                </div>
              </li>
              <li>
                <div class="treeview-animated-element">
                  <i class="fas fa-tasks ic-w mr-1"></i>Yamato
                </div>
              </li>
              <li>
                <div class="treeview-animated-element">
                  <i class="fas fa-tasks ic-w mr-1"></i>SEUR
                </div>
              </li>
            </ul>
          </li>
        </ul>

        <ul class="nested">
          <li class="treeview-animated-items">
            <a class="closed">
              <i class="fas fa-angle-right"></i>
              <span>
                <i class="fas fa-flag ic-w mx-1"></i>Project work
              </span>
            </a>
            <ul class="nested">
              <li>
                <div class="treeview-animated-element">
                  <i class="fas fa-tasks ic-w mr-1"></i>Search Shipment
                </div>
              </li>
              <li>
                <div class="treeview-animated-element">
                  <i class="fas fa-tasks ic-w mr-1"></i>Expected Events
                </div>
              </li>
              <li>
                <div class="treeview-animated-element">
                  <i class="fas fa-tasks ic-w mr-1"></i>Change Request - TrackAndTraceXML Report
                </div>
              </li>
              <li>
                <div class="treeview-animated-element">
                  <i class="fas fa-tasks ic-w mr-1"></i>WMS Integration
                </div>
              </li>
              <li>
                <div class="treeview-animated-element">
                  <i class="fas fa-tasks ic-w mr-1"></i>Project work
                </div>
              </li>
            </ul>
          </li>
        </ul>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "TaskList",
  props: {
    msg: String,
    yourName: String,
  },
};
</script>

<style scoped>
.treeview-animated.w-20 {
  width: 20rem;
  font-size: 14px;
}

.treeview-animated h6 {
  font-size: 1.4em;
}

.treeview-animated ul {
  position: relative;
  list-style: none;
  padding-left: 1em;
}

.treeview-animated-list li {
  padding: 0.2em 0 0 0.2em;
}

.treeview-animated-element {
  padding: 0.2em 0.2em 0.2em 0.6em;
  cursor: pointer;
  transition: all 0.1s linear;
  border-bottom-left-radius: 4px;
  border-top-left-radius: 4px;
}

.treeview-animated-element:hover {
  background-color: rgb(140, 185, 255);
}

.treeview-animated-element.opened {
  color: #f8f9fa;
  background-color: rgb(50, 160, 255);
}

.treeview-animated-element.opened:hover {
  color: #f8f9fa;
  background-color: rgb(50, 160, 255);
}

.treeview-animated-items .nested::before {
  content: "";
  display: block;
  position: absolute;
  background-color: grey;
  left: 5px;
  width: 5px;
  height: 100%;
}

.treeview-animated-items .closed {
  display: block;
  padding: 0.2em 0.2em 0.2em 0.4em;
  margin-right: 0;
  border-top-left-radius: 0.3em;
  border-bottom-left-radius: 0.3em;
}

.treeview-animated-items .closed:hover {
  background-color: rgb(140, 185, 255);
}

.treeview-animated-items .open {
  transition: all 0.1s linear;
  background-color: rgb(50, 160, 255);
}

.treeview-animated-items .open span {
  color: #f8f9fa;
}

.treeview-animated-items .open:hover {
  color: #f8f9fa;
  background-color: rgb(50, 160, 255);
}

.treeview-animated ul li .open div:hover {
  background-color: rgb(50, 160, 255);
}

.treeview-animated-items .closed .fa-angle-right {
  transition: all 0.1s linear;
  font-size: 0.8rem;
}

.closed .fa-angle-right.down {
  position: relative;
  color: #f8f9fa;
  transform: rotate(90deg);
}
</style>