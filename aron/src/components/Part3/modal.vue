<template>
  <transition name="modal-fade">
    <div id="modal_container">
    <div class="modal-backdrop">
      <div class="Myform">
        <h1>Request Demo</h1>
        <div class="inp">
          <form name="regisrration" action="form.php" method="post" style="
    background: none">
            <input class="log" type="text" required placeholder="Name" name="login" />
            <input
              class="pass"
              type="email"
              required
              placeholder="Email"
              name="password"
            />
            <div class="info">
              <a href="#" @click="close">Close</a>
            </div>
            <input class="btn" type="submit" value="Request" />
          </form>
        </div>
      </div>
    </div>
    </div>
  </transition>
</template>

<script lang="ts">
export default {
  name: "modalWindow",
  methods: {
    close() {
    
      this.$emit("close");
    },
  },
};
</script>
<style>
@import '../styles/modal.css';
</style>
