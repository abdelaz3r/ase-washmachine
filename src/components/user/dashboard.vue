<template>
  <div>
    <dashboard :display="display">
      <div slot="title">
        User Dashboard
      </div>
      <div class="columns">
        <div class="column">
          <a href="#/user/launch-cycle">
            <div class="notification is-warning subtitle is-4">Launch a cycle</div>
          </a>
        </div>
        <div class="column">
          <a href="#/user/settings" >
            <div class="notification is-secondary subtitle is-4">Settings</div>
          </a>
        </div>
        <div class="column">
          <a href="#/user/user-analytics" >
            <div class="notification is-primary subtitle is-4">Analytics</div>
          </a>
        </div>
      </div>
    </dashboard>
  </div>
</template>

<script>
export default {
  data: function() {
    return {
      display: false
    }
  }
}
</script>

<style>
.notification {
  text-align: center;
}

.notification.is-warning {
  color: white;
}

.panel {
  padding-top: 10vh;
}

.columns {
  width: 100%
}
</style>