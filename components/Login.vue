<template>
  <div class="d-flex flex-column flex-root">
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
                  <div class="pb-5 pb-lg-15">
                      <h3 class="font-weight-bolder text-dark font-size-h2 font-size-h1-lg">Sign In</h3>
                  </div>
                  <!--begin::Title-->
                  <div class="mb-5 form-group">
                      <input id="email" type="email" class="h-auto px-6 border-0 rounded-lg form-control form-control-solid py-7" name="email" placeholder="Email" required autocomplete="email" autofocus>
                      <span class="invalid-feedback" role="alert">
                          <strong></strong>
                      </span>
                  </div>
                  <div class="mb-5 form-group">
                      <input id="password" type="password" class="h-auto px-6 border-0 rounded-lg form-control form-control-solid py-7" name="password" placeholder="Password" required autocomplete="current-password">
                          <span class="invalid-feedback" role="alert">
                              <strong></strong>
                          </span>
                  </div>
                  <div class="flex-wrap form-group d-flex justify-content-between align-items-center">
                      <div class="checkbox-inline">
                          <label class="m-0 checkbox text-muted">
                          <input type="checkbox" name="remember" />
                          <span></span>Remember me</label>
                      </div>
                      <nuxt-link to="forget" class="text-muted text-hover-primary">Forget Password ?</nuxt-link>
                  </div>
                  <!--begin::Action-->
                  <div class="pb-5 pb-lg-0">
                      <nuxt-link to="dashboard" class="px-8 py-4 my-3 mr-3 btn btn-primary font-weight-bolder font-size-h6">Sign In</nuxt-link>
                  </div>
                  <!--end::Action-->
              </form>
              <div class="mt-10">
                  <span class="mr-4 opacity-70">Don't have an account yet?</span>
                  <nuxt-link to="register" class="text-muted text-hover-danger font-weight-bold">Create Account</nuxt-link>
              </div>
          </div>
          <!--end::Login Sign in form-->
      </div>
      </div>
    </div>
    <!--end::Login-->
  </div>
</template>
