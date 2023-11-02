<template>
  <main class="auth-page">
    <div class="container-page">
      <div class="row">
        <div class="col-md-6 offset-md-3 col-xs-12">
          <h1 class="text-xs-center">Sign Up</h1>
          <p class="text-xs-center"></p>
          <router-link :to="{ name: 'login' }">Need new account?</router-link>
          VALIDATION ERRORS
          <form @submit.prevent="onSubmit">
            <fieldset class="form-group">
              <input
                type="text"
                class="form-control form-control-lg"
                placeholder="Username"
              />
            </fieldset>
            <fieldset class="form-group">
              <input
                type="text"
                class="form-control form-control-lg"
                placeholder="Email"
              />
            </fieldset>
            <fieldset class="form-group">
              <input
                type="password"
                class="form-control form-control-lg"
                placeholder="Password"
              />
            </fieldset>
            <button class="btn btn-primary btn-lg pull-xs-right">
              Sign Up
            </button>
          </form>
        </div>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: 'compRegister',
  methods: {
    onSubmit() {
      console.log('Submitted Form');
    },
  },
};
</script>
