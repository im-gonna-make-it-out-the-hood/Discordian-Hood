<svelte:head>
<style>


  .login-container {
    width: 300px;
    padding: 16px;
    background-color: #fff;
    margin: 0 auto;
    margin-top: 250px;
    border-radius: 8px;
  }



  .discord-button {
    width: 100%;
    padding: 10px;
    border-radius: 5px;
    border: none;
    color: #232222;
    background-color: #7289da;
    cursor: pointer;
    transition: background-color 0.3s ease;
    margin-top: 10px;
  }

  .discord-button:hover {
    background-color: #7289da61;
  }

  body {
      background: #333;
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
    }

    .container {
      max-width: 800px;
      margin: 0 auto;
      padding: 20px;
    }
    </style>
    </svelte:head>
    <div class="login-container">
        <button class="discord-button" type="submit">Log in with Discord</button>
      </div>