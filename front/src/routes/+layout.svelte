<script>
    import '../app.css'; 
  </script>
  
  <!-- transparent navbar -->
  <nav class="navbar">
    <div class="logo text-white text-xl font-bold hover:text-yellow-400">
      6XH
    </div>
  
    <button
      class="menu-btn"
      on:click="{() => console.log('Menu clicked')}"
      aria-label="Toggle menu"
    >
      <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
        <path d="M3 12h18M3 6h18M3 18h18"/>
      </svg>
    </button>
  </nav>
  
  <slot></slot>
  
  <style>

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
      background-color: rgba(0, 0, 0, 0.4); 
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
  
    .menu-btn svg {
      fill: white; 
    }
  </style>
  