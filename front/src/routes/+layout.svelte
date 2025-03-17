<script>
    import '../app.css'; 
  </script>
  
  <!-- transparent navbar -->
  <nav class="navbar">
    <a href="/">
      <div class="logo text-white text-xl font-bold hover:text-blue-500 menu-btn">
        <img class="svg-icon" src="/src/assets/svg/symbols/home-symbol-black-256px.svg" alt="logo" />
      </div>
    </a>
    <a href="https://github.com/toastinthetub">
      <div class="logo text-white text-xl font-bold hover:text-blue-500 menu-btn">
        <img class="svg-icon" src="src/assets/svg/symbols/github-black-256px.svg" alt="logo" />
      </div>
    </a>
  </nav>
<footer style="position: fixed; bottom: 0; width: 100%; background: black; padding: 10px 0; text-align: center;">
  <a href="/" style="color: white; text-decoration: none; font-weight: bold; color: #EB5E28">HOME</a>
</footer>
  
  <slot></slot>
  
  <style>

    .svg-icon {
      width: 32px;
      height: 32px;
    }

    .logo:hover {
      text-shadow: 0 0 10px rgba(255, 255, 255, 0.7); 
    }
  
    .navbar {
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      padding: 1rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      background-color: #ccc5b9;
      backdrop-filter: blur(10px); 
      z-index: 10; 
    }
  
    .menu-btn {
      width: 36px;
      height: 36px;
      cursor: pointer;
      background: whitesmoke;
      border-radius: 100%;
      border: none; 
    }
  
    .menu-btn img {
      fill: white; 
    }
  </style>
  