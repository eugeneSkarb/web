  <template>
    <div>
      <div class="login-container">
        <h1>Вход</h1>
        <p>Пожалуйста, заполните поля, чтобы войти в свой аккаунт.</p>
        <hr>

        <h3>E-mail</h3>
        <input class="input-field" type="text" placeholder="Введите E-mail" name="email" required>

        <h3>Пароль</h3>
        <input class="input-field" type="password" placeholder="Введите пароль" name="psw" required>
        <hr>

        <button type="submit" class="loginbtn">Войти</button>

        <div class="regist">
          <p>Еще нет аккаунта? Бегом создавать! <router-link :to="{name: 'Registration'}">Зарегистрироваться</router-link>.</p>
        </div>
      </div>
    </div>
  </template>

  <script>
  export default {
    name: "Login"
  }
  </script>

  <style scoped>
    .login-container {
      display: flex;
      flex-direction: column;
      background-color: white;
      position: relative;
      width: 30%;
      margin-left: 400px;
      margin-top: 100px;
      padding: 20px;
      font-size: 20px;
      box-shadow: rgb(255 255 255) 2px 2px 2px;
    }

    .login-container h1 {
      margin-bottom: 15px;
    }

    .loginbtn {
      background-color: darkred;
      color: white;
      padding: 16px 20px;
      margin: 8px 0;
      border: none;
      cursor: pointer;
      opacity: 0.9;
      font-size: 20px;
    }

    .loginbtn:hover {
      opacity: 1;
    }

    .login-container h3 {
      padding-top: 15px;
    }

    .regist {
      display: flex;
      justify-content: center;
      align-items: center;
      margin-top: 20px;
      background: #f1f1f1;
      min-height: 50px;
      font-size: 20px;
    }

    .regist a{
      color: #636365;
    }

    .regist a:hover {
      font-weight: bold;
      color: darkred;
    }

    .input-field {
      padding: 15px;
      margin: 5px 0 22px 0;
      display: inline-block;
      border: none;
      background: #f1f1f1;
      font-size: 15px;
    }

    .input-field:focus {
      background-color: #ddd;
      outline: none;
    }
  </style>