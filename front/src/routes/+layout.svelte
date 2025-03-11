<script>
    import '../app.css'; 
  </script>
  
  <!-- transparent navbar -->
  <nav class="navbar">
    <a href="/">
      <div class="logo text-white text-xl font-bold hover:text-blue-500">
        <img class="svg-icon" src="https://www.svgrepo.com/show/535439/home-1.svg" alt="logo" />
      </div>
    </a>
    <a href="https://github.com/toastinthetub">
      <div class="logo text-white text-xl font-bold hover:text-blue-500">
        <img class="svg-icon" src="https://www.svgrepo.com/show/512317/github-142.svg" alt="logo" />
      </div>
    </a>
  </nav>4
  
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
      width: 30px;
      height: 30px;
      cursor: pointer;
      background: none; 
      border: none; 
    }
  
    .menu-btn img {
      fill: white; 
    }
  </style>
  