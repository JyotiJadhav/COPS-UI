<template>
  <div v-if="showModal" id="addTemplate">
    <transition name="modal fade" role="dialog">
      <div class="modal-backdrop">
        <div
          class="modal-dialog modal-dialog-centered"
          style="max-width: 600px !important"
          role="document"
        >
          <div class="modal-content">
            <div class="modal-header">
              <h2 class="modal-title">Add Template</h2>
              <button
                type="button"
                class="close"
                data-dismiss="modal"
                aria-label="Close"
              >
                <span aria-hidden="true">&times;</span>
              </button>
            </div>
            <div class="modal-body">
              <AddTemplate></AddTemplate>
            </div>
            <div class="modal-footer">
              <button type="button" class="btn btn-primary">
                Save changes
              </button>
              <button
                type="button"
                class="btn btn-secondary"
                data-dismiss="modal"
                @click="hide"
              >
                Close
              </button>
            </div>
          </div>
        </div>
      </div>
    </transition>
  </div>
</template>


<script>
import AddTemplate from "../Template/AddTemplate";
export default {
  // name: "AddTemplateModal",
  components: { AddTemplate },

  data() {
    return {
      showModal: false,
    };
  },
  methods: {
    show() {
      this.showModal = true;
    },
    hide() {
      this.showModal = false;
    },
  },
};
</script>

