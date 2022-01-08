  <template>
    <div id="app">
      <header>
        <h1> Breaking news</h1>
        <hr>
          <nav>
            <ul>
              <li>
                <router-link :to="{name: 'Home'}">Главная</router-link>
              </li>
              <li>
                <router-link :to="{name: 'About'}">Игры</router-link>
              </li>
              <li>
                <router-link :to="{name: 'About'}">Политика</router-link>
              </li>
              <li>
                <router-link :to="{name: 'About'}">Спорт</router-link>
              </li>
              <li>
                <router-link :to="{name: 'About'}">О нас</router-link>
              </li>
              <div class="authorization">
                <li>
                  <router-link :to="{name: 'Registration'}" class="registration">Регистрация</router-link>
                </li>
                <li>
                  <router-link :to="{name: 'Login'}" class="login">Вход</router-link>
                </li>
              </div>
            </ul>
          </nav>
      </header>

      <router-view />

      <footer>
        <hr>
        <p>"ООО Крутая Газета"</p>
        <p>тел. +7-930-853-37-02</p>
      </footer>
    </div>
  </template>

  <style>
    * {
      margin: 0;
      padding: 0
    }

    body {
      background-size: cover;
      background-repeat: no-repeat;
      background-position: center;
      width: 100%;
      height: 100%;
      background-image: url("https://flytothesky.ru/wp-content/uploads/2017/09/3321.jpg");
      background-attachment: fixed;
      font-family: 'Roboto Condensed', sans-serif;
    }
    header {
      width: 250px;
      border: 1px solid white;
      padding-left: 10px;
      position: fixed;
      left: 0;
      top: 0;
    }

    header h1{
      font-size: 60px;
      color: darkred;
      font-weight: bold;
    }

    nav ul {
      margin-top: 5vh;
      display: inline-block;
    }

    nav ul li a {
      text-decoration: none;
      color: white;
      font-size: 20px;
      font-weight: bold;
    }

    nav ul li a:hover {
      color:darkred;
    }

    nav ul li {
      list-style-type: none;
      padding-bottom: 5vh;
    }

    footer {
      width: 20%;
      margin-top: auto;
      position: fixed;
      bottom: 0;
      left: 0;
    }

    footer p {
      padding-top: 10px;
      padding-left: 10px;
      font-size: 15px;
      font-style: italic;
      color: white;
    }

    .login {
      margin-left: 30px;
      border: 2px solid rgba(255, 255, 255, 0.49);
      padding: 5px;
      border-radius: 7px;
      color: rgba(255, 255, 255, 0.49);
    }

    .registration {
      border: 2px solid rgba(255, 255, 255, 0.49);
      padding: 5px;
      border-radius: 7px;
      color: rgba(255, 255, 255, 0.49);
    }

    .login:hover {
      background-color: rgba(255, 255, 255, 0.18);
      color: white;
    }

    .registration:hover {
      background-color: rgba(255, 255, 255, 0.18);
      color: white;
    }

    .authorization {
      display: flex;
      flex-direction: row;
      margin-top: 30px;
    }

  </style>
