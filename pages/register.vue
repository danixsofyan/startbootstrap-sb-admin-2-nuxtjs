<template>
  <!--begin::Login-->
    <div class="login login-4 login-signin-on d-flex flex-row-fluid" id="kt_login">
      <div class="d-flex flex-center flex-row-fluid bgi-size-cover bgi-position-top bgi-no-repeat" style="background-image: url('/bg-auth.jpg');">
        <div class="overflow-hidden text-center login-form p-7 position-relative">
          <!--begin::Login Header-->
          <div class="d-flex flex-center mb-15">
            <a href="index.html">
              <img src="/logo-indigo.png" class="max-h-75px" alt="" />
            </a>
          </div>
          <!--end::Login Header-->
          <!--begin::Login Sign in form-->
          <div class="login-signin">
              <form method="POST" class="form" id="kt_login_signin_form">
                  <!--begin::Title-->
                  <div class="pb-10 pb-lg-12">
                      <h3 class="font-weight-bolder text-dark font-size-h2 font-size-h1-lg">Create Account</h3>
                      <div class="text-muted font-weight-bold font-size-h4">
                          Already have an Account ?
                          <nuxt-link to="login" class="text-danger font-weight-bolder">Sign In</nuxt-link>
                      </div>
                  </div>
                  <!--begin::Form group-->
                  <div class="form-group">
                      <input id="name" type="text" class="h-auto px-6 border-0 rounded-lg form-control form-control-solid py-7" name="name" value="" placeholder="Name" required autocomplete="name" autofocus>
                          <!-- <span class="invalid-feedback" role="alert">
                              <strong>{{ $message }}</strong>
                          </span> -->
                  </div>
                  <!--end::Form group-->

                  <!--begin::Form group-->
                  <div class="form-group">
                      <input id="email" type="email" class="h-auto px-6 border-0 rounded-lg form-control form-control-solid py-7" name="email" value="" placeholder="Email" required autocomplete="email">
                          <!-- <span class="invalid-feedback" role="alert">
                              <strong>{{ $message }}</strong>
                          </span> -->
                  </div>
                  <!--end::Form group-->

                  <!--begin::Form group-->
                  <div class="form-group">
                      <input id="password" type="password" class="h-auto px-6 border-0 rounded-lg form-control form-control-solid py-7" name="password" placeholder="Password" required autocomplete="new-password">
                          <!-- <span class="invalid-feedback" role="alert">
                              <strong>{{ $message }}</strong>
                          </span> -->
                  </div>
                  <!--end::Form group-->

                  <!--begin::Form group-->
                  <div class="form-group">
                      <input id="password-confirm" type="password" class="h-auto px-6 border-0 rounded-lg form-control form-control-solid py-7" name="password_confirmation" placeholder="Confirm Password" required autocomplete="new-password">
                  </div>
                  <!--end::Form group-->

                  <!--begin::Action-->
                  <div class="pb-5 pb-lg-0">
                      <button type="submit" id="kt_login_singin_form_submit_button" class="px-8 py-4 my-3 mr-3 btn btn-primary font-weight-bolder font-size-h6">Register</button>
                  </div>
                  <!--end::Action-->
              </form>
          </div>
          <!--end::Login Sign in form-->
      </div>
      </div>
    </div>
    <!--end::Login-->
</template>

<script>
export default {
  layout : 'auth'
}
</script>
