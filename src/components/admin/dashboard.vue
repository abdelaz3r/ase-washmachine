<template>
  <div>
    <dashboard :display="display">
      <div slot="title">
        Admin Dashboard
      </div>
      <div class="columns">
        <div class="column">
          <a href="#/admin/users">
            <div class="notification is-info subtitle is-4">
              Users
            </div>
          </a>
        </div>
        <div class="column">
          <a href="#/admin/machines" >
            <div class="notification is-warning subtitle is-4">Machines</div>
          </a>
        </div>
        <div class="column">
          <router-link class="notification is-danger is-4 subtitle" :to="{ name: 'programs' }">Programs</router-link>
        </div>
        <div class="column">
          <a href="#/admin/statistics">
            <div class="notification is-primary subtitle is-4">Statistics</div>
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
  },
  mounted() {

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
