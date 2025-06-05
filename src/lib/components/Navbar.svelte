<script lang="ts">
  // menuOpen and toggleMenu are used in the markup for the hamburger menu
  let menuOpen = false;
  function toggleMenu() {
    menuOpen = !menuOpen;
  }
</script>

<nav>
  <ul class="desktop-menu">
    <li>
      <a href="/">
        <svg width="20" height="20" fill="none" stroke="#64ffda" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24" style="vertical-align: middle; margin-right: 0.4rem;"><path d="M3 12L12 3l9 9"/><path d="M9 21V9h6v12"/></svg>
        Home
      </a>
    </li>
    <li>
      <a href="/skills">
        <svg width="20" height="20" fill="none" stroke="#64ffda" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24" style="vertical-align: middle; margin-right: 0.4rem;"><rect x="2" y="6" width="20" height="12" rx="2"/><path d="M6 10h.01M10 10h.01M14 10h.01M18 10h.01M6 14h12"/></svg>
        Skills
      </a>
    </li>
    <li>
      <a href="/contact">
        <svg width="20" height="20" fill="none" stroke="#64ffda" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24" style="vertical-align: middle; margin-right: 0.4rem;"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="M22 6 12 13 2 6"/></svg>
        Contact
      </a>
    </li>
  </ul>
  <button class="hamburger" on:click={toggleMenu} aria-label="Open menu">
    <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="#64ffda" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
      <line x1="3" y1="6" x2="21" y2="6"/>
      <line x1="3" y1="12" x2="21" y2="12"/>
      <line x1="3" y1="18" x2="21" y2="18"/>
    </svg>
  </button>
  {#if menuOpen}
    <div
      class="mobile-menu-overlay"
      role="dialog"
      tabindex="0"
      on:keydown={(e) => {
        if (e.key === 'Escape') menuOpen = false;
      }}
    >
      <div class="mobile-menu-wrapper" role="presentation" tabindex="-1" on:keydown={(e) => { if (e.key === 'Escape') menuOpen = false; }}>
        <ul class="mobile-menu">
          <li>
            <a href="/" on:click={() => (menuOpen = false)}>
              <svg width="20" height="20" fill="none" stroke="#64ffda" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24" style="vertical-align: middle; margin-right: 0.4rem;"><path d="M3 12L12 3l9 9"/><path d="M9 21V9h6v12"/></svg>
              Home
            </a>
          </li>
          <li>
            <a href="/skills" on:click={() => (menuOpen = false)}>
              <svg width="20" height="20" fill="none" stroke="#64ffda" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24" style="vertical-align: middle; margin-right: 0.4rem;"><rect x="2" y="6" width="20" height="12" rx="2"/><path d="M6 10h.01M10 10h.01M14 10h.01M18 10h.01M6 14h12"/></svg>
              Skills
            </a>
          </li>
          <li>
            <a href="/contact" on:click={() => (menuOpen = false)}>
              <svg width="20" height="20" fill="none" stroke="#64ffda" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24" style="vertical-align: middle; margin-right: 0.4rem;"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="M22 6 12 13 2 6"/></svg>
              Contact
            </a>
          </li>
        </ul>
      </div>
    </div>
  {/if}
</nav>

<style>
nav {
  background: #0a192f;
  padding: 1rem 1.5rem; 
  display: flex; 
  justify-content: space-between; 
  align-items: center;
  position: relative; 
}

/* Desktop Menu */
.desktop-menu {
  display: flex; 
  gap: 3.5rem;
  list-style: none;
  margin: 0;
  padding: 0;
  width: 100%; 
  justify-content: center;

}

/* Hamburger */
.hamburger {
  display: none;
  background: none;
  border: none;
  cursor: pointer;
  position: fixed;
  right: 1.5rem;
  top: 1rem;
  z-index: 10000;
  overflow: hidden;
}

.mobile-menu-overlay {
  display: none; 
}

li a {
  color: #64ffda;
  text-decoration: none;
  font-weight: bold;
  font-size: 1.2rem;
  transition: color 0.2s;
  display: flex;
  align-items: center;
}
li a:hover {
  color: #fff;
}
li a svg {
  transition: stroke 0.2s;
}
li a:hover svg {
  stroke: #fff;
}

/* Mobile styles */
@media (max-width: 700px) {
  .desktop-menu {
    display: none; 
  }

  .hamburger {
    display: block;
  }

  nav {
    padding: 2rem 0;
  }

  .mobile-menu-overlay {
    position: fixed;
    inset: 0; 
    width: 100vw;
    height: 100vh;
    background: #0a192f;
    z-index: 9999;
    display: flex;
    align-items: center;
    justify-content: center;
    pointer-events: auto;
  }

  .mobile-menu-wrapper {
    display: flex;
    flex-direction: column;
    align-items: center; 
    width: 100vw;
    background-color: #0a192f; /* Match overlay and page background */
    padding: 2rem 0;
    left: 0;
    right: 0;
    border-radius: 0;
    pointer-events: auto;
  }

  .mobile-menu {
    display: flex;
    flex-direction: column;
    align-items: center; 
    gap: 2.5rem;
    font-size: 1.5rem;
    width: 100%;
    list-style: none !important; 
    padding: 0 !important;
    margin: 0 !important; 
  }

  .mobile-menu li {
    margin: 0;
    padding: 0;
    list-style: none !important; 
  }

  .mobile-menu li a {
    color: #64ffda;
    font-weight: bold;
    font-size: 1.5rem;
    text-decoration: none;
    display: flex;
    align-items: center;
    transition: color 0.2s;
    cursor: pointer;
  }
  .mobile-menu li a:hover {
    color: #fff;
  }
}
</style> 