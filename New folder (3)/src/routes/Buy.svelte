<svelte:head>
  <style>
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

    .header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 20px;
    }

    .logo {
      font-size: 1.8em;
      font-weight: bold;
      color: white;
    }

    .tabs {
      display: flex;
    }

    .tab {
      padding: 10px 20px;
      background-color: #1976d2;
      color: white;
      font-size: 1.2em;
      font-weight: bold;
      text-decoration: none;
      margin-right: 10px;
      border-radius: 5px;
      transition: background-color 0.3s;
    }

    .tab:hover {
      background-color: #135699;
    }

    .content {
      background-color: #f2f2f2;
      padding: 20px;
      border-radius: 5px;
      color: #333;
    }

    .product {
      display: flex;
      align-items: center;
      margin-bottom: 20px;
      padding: 10px;
      background-color: #f2f2f2;
      border-radius: 5px;
      color: #333;
    }

    .product img {
      width: 100px;
      height: 100px;
      object-fit: cover;
      margin-right: 10px;
    }

    .product .info {
      flex: 1;
    }

    .product .title {
      font-size: 1.2em;
      font-weight: bold;
      margin-bottom: 5px;
    }

    .product .price {
      font-size: 1em;
      color: #1976d2;
      margin-bottom: 5px;
    }

    .product .description {
      font-size: 0.9em;
      color: #666;
    }

    .column1 {
      margin-top: 50px;
    }

    .column1 h2 {
      font-size: 1.8em;
      font-weight: bold;
      margin-bottom: 10px;
    }

    .column1 p {
      font-size: 1.2em;
      margin-bottom: 10px;
    }

    .sellix-button2 {
      margin-top: 20px;
    }

    .sellix-button2 a {
      padding: 15px 32px;
      text-align: center;
      font-size: 16px;
      font-weight: 900;
      cursor: pointer;
      border-style: solid;
      border-color: #fff;
      border-width: 1px;
      border-radius: 5px;
      background-color: transparent;
      color: #fff;
      text-decoration: none;
      transition: background-color 0.3s;
    }

    
  </style>
</svelte:head>


<div class="container">

<div class="content">
<!-- Product listings -->
<div class="product">
  <!-- svelte-ignore a11y-img-redundant-alt -->
  <img src="https://media.discordapp.net/attachments/1084256527180898324/1141923633137205339/toolbox.png?width=125&height=125" alt="Product Image" />
  <div class="info">
    <div class="title">Auto Bypasser Bot</div>
    <div class="price">$5</div>
    <div class="description">The best & most highest quality product in the community.</div>
  </div>
</div>

<!-- Product section -->
<div class="column1">
  <h2>Discordian Hood | Auto Bypasser Bot</h2>
  <p>The #1 most helpful tool for bypassing!</p>
  <div class="sellix-button2">
    <a href="#" style="padding: 15px 32px; text-align: center; font-size: 16px; font-weight: 900; cursor: pointer; border-style: solid; border-color: lightgrey; border-width: 1px; border-radius: 5px; background-color: #9370DB; color: white;">Purchase</a>
  </div>
</div>

</div>
</div>
