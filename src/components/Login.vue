<template>
  <div class="login">
    <h1>LOGIN</h1>
    <div class="form">
      <form>
        <div class="form-box">
          <input type="text" placeholder="Email or user name" />
        </div>
        <div class="form-box">
          <input type="password" placeholder="Password" />
        </div>
        <div class="flex-container">
          <div class="toggle">
            <label class="switch">
              <input class="slider" type="checkbox" checked />
              <span class="slider round"></span>
            </label>
            <spam class="aux">Remember me</spam>
          </div>
          <div>
            <a class="aux" href="#">Forgot Password</a>
          </div>
        </div>
        <input class="submit" type="submit" value="Login" />
      </form>
      <p>OR</p>
      <p class="oppaco">Login / Sing up with</p>
      <div class="flex-container-social-media">
        <div>
          <a href="#" id="facebook">
            <font-awesome-icon :icon="{ prefix: 'fab', iconName: 'facebook-f' }" />
          </a>
        </div>
        <div>
          <a href="#" id="google">
            <font-awesome-icon :icon="{ prefix: 'fab', iconName: 'google' }" />
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
* {
  color: #000;
}

.login {
  padding: 20px; /* borda interna geral */
  background-color: #fff;
  border-radius: 15px;
  height: 400px;
  width: 350px;
  box-shadow: 0 6px 3px rgba(0, 0, 0, 0.16), 0 6px 3px rgba(0, 0, 0, 0.23);
}

.login h1 {
  text-align: left;
  font-size: 1.5em;
  margin: 5px;
}

.form-box input {
  width: 95%;
  height: 40px;
  border-radius: 5px;
  margin-top: 20px;
  border-color: #0002;
  padding-left: 5px; /* borda interna esquerda */
}

.form-box input:focus, textarea:focus {
    outline: none;
    border:2px solid #719ECE;
    box-shadow: 0 0 5px #719ECE;
}

.submit {
  width: 200px;
  height: 35px;
  border-radius: 5px;
  margin-top: 10px;
  background-color: #ff538d;
  color: #fff;
  border: none;
  box-shadow: 0 3px 6px rgba(0, 0, 0, 0.16), 0 3px 6px rgba(0, 0, 0, 0.23);
}

.submit:hover {
  background-color: #d33e70;
}

.submit:focus{
    outline: none;
    box-shadow: 0 0 6px #719ECE;
    background-color: #d33e70;
}

.oppaco {
  color: #8b8b8b;
  font-size: 0.8em;
}

.toggle{
    display:inline-block;
}

.switch {
  position: relative;
  display: inline-block;
  width: 30px;
  height: 16px;
}

.switch input {
  opacity: 0;
  width: 0;
  height: 0;
}

.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #ccc;
  -webkit-transition: 0.4s;
  transition: 0.4s;
}

.slider:before {
  position: absolute;
  content: "";
  height: 12px;
  width: 12px;
  left: 2px;
  bottom: 2px;
  background-color: white;
  -webkit-transition: 0.4s;
  transition: 0.4s;
}

input:checked + .slider {
  background-color: #2196f3;
}

input:focus + .slider {
  box-shadow: 0 0 1px #2196f3;
}

input:checked + .slider:before {
  -webkit-transform: translateX(13px);
  -ms-transform: translateX(13px);
  transform: translateX(13px);
}

/* Rounded sliders */
.slider.round {
  border-radius: 16px;
}

.slider.round:before {
  border-radius: 50%;
}

.aux {
  font-size: 0.75em;
  color: #000;
  margin-left: 5px;
}

a {
  text-decoration: none;
}

.flex-container {
  display: flex;
  width: 90%;
  justify-content: space-between;
  margin: 0 auto;
  margin-top: 10px;
}

.flex-container-social-media {
  display: flex;
  width: 30%;
  justify-content: space-between;
  margin: 0 auto;
}
</style>