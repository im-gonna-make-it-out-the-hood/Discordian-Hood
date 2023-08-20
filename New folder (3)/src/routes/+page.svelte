<svelte:head>
<style>


  .login-container {
    width: 300px;
    padding: 16px;
    background-color: #34495e;
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
    .tab.active {
      background-color: #135699;
    }
</style>
</svelte:head>
  
  <div class="container">
    <div class="header">
      <div class="logo">Discordian Hood</div>
      <div class="tabs">
        <a href="#" class="tab {activeTab === 'home' ? 'active' : ''}" on:click={() => changeTab('home')}>Home</a>
        <a href="#" class="tab {activeTab === 'buy' ? 'active' : ''}" on:click={() => changeTab('buy')}>Buy</a>
        <a href="#" class="tab {activeTab === 'feedback' ? 'active' : ''}" on:click={() => changeTab('feedback')}>Feedback</a>
        <a href="#" class="tab {activeTab === 'tos' ? 'active' : ''}" on:click={() => changeTab('tos')}>ToS</a>
      </div>
    </div>
  </div>
  
  
  

  
  {#if activeTab === 'buy'}
    <Buy />
  {/if}
  
  {#if activeTab === 'home'}
    <Home />
  {/if}
  {#if activeTab === 'tos'}
    <TOS />
  {/if}

  <script>
     let activeTab = 'home';
  
  const changeTab = (/** @type {string} */ tab) => {
    activeTab = tab;
  };
  // @ts-ignore
    import Home from './Home.svelte';
    import Buy from './Buy.svelte';
    import Feedback from './Feedback.svelte';
    import TOS from './TOS.svelte';
  </script>