<script lang="ts">
  // No logic needed for now
</script>

<footer class="main-footer">
  <div class="footer-content">
    <div class="footer-links">
      <a href="mailto:1124abdul@gmail.com" class="footer-link" title="Email">
        <svg width="24" height="24" fill="none" stroke="#64ffda" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="M22 6 12 13 2 6"/></svg>
        <span>Email</span>
      </a>
      <a href="https://www.linkedin.com/in/abdul-qadeer-4bba17168/" class="footer-link" target="_blank" rel="noopener noreferrer" title="LinkedIn">
        <svg width="24" height="24" fill="none" stroke="#64ffda" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><rect x="2" y="2" width="20" height="20" rx="5"/><path d="M16 8a6 6 0 0 1 6 6v6"/><circle cx="8.5" cy="8.5" r="1.5"/><path d="M6 20v-7"/><path d="M12 20v-4a2 2 0 0 1 2-2h2"/></svg>
        <span>LinkedIn</span>
      </a>
      <a href="https://github.com/A-Qadeer542" class="footer-link" target="_blank" rel="noopener noreferrer" title="Personal GitHub">
        <svg width="24" height="24" fill="none" stroke="#64ffda" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12c0 4.42 2.87 8.17 6.84 9.5.5.09.66-.22.66-.48v-1.7c-2.78.6-3.37-1.34-3.37-1.34-.45-1.15-1.1-1.46-1.1-1.46-.9-.62.07-.61.07-.61 1 .07 1.53 1.03 1.53 1.03.89 1.52 2.34 1.08 2.91.83.09-.65.35-1.08.63-1.33-2.22-.25-4.56-1.11-4.56-4.95 0-1.09.39-1.98 1.03-2.68-.1-.25-.45-1.27.1-2.65 0 0 .84-.27 2.75 1.02A9.56 9.56 0 0 1 12 6.8c.85.004 1.71.11 2.51.32 1.91-1.29 2.75-1.02 2.75-1.02.55 1.38.2 2.4.1 2.65.64.7 1.03 1.59 1.03 2.68 0 3.85-2.34 4.7-4.57 4.95.36.31.68.92.68 1.85v2.75c0 .27.16.58.67.48A10.01 10.01 0 0 0 22 12c0-5.52-4.48-10-10-10z"/></svg>
        <span>Personal GitHub</span>
      </a>
      <a href="https://github.com/A-Qadeer142" class="footer-link" target="_blank" rel="noopener noreferrer" title="Work GitHub">
        <svg width="24" height="24" fill="none" stroke="#64ffda" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12c0 4.42 2.87 8.17 6.84 9.5.5.09.66-.22.66-.48v-1.7c-2.78.6-3.37-1.34-3.37-1.34-.45-1.15-1.1-1.46-1.1-1.46-.9-.62.07-.61.07-.61 1 .07 1.53 1.03 1.53 1.03.89 1.52 2.34 1.08 2.91.83.09-.65.35-1.08.63-1.33-2.22-.25-4.56-1.11-4.56-4.95 0-1.09.39-1.98 1.03-2.68-.1-.25-.45-1.27.1-2.65 0 0 .84-.27 2.75 1.02A9.56 9.56 0 0 1 12 6.8c.85.004 1.71.11 2.51.32 1.91-1.29 2.75-1.02 2.75-1.02.55 1.38.2 2.4.1 2.65.64.7 1.03 1.59 1.03 2.68 0 3.85-2.34 4.7-4.57 4.95.36.31.68.92.68 1.85v2.75c0 .27.16.58.67.48A10.01 10.01 0 0 0 22 12c0-5.52-4.48-10-10-10z"/></svg>
        <span>Work GitHub</span>
      </a>
    </div>
    <div class="footer-copyright">
      &copy; {new Date().getFullYear()} Abdul Qadeer. All rights reserved.
    </div>
  </div>
</footer>

<style>
.main-footer {
  background: #0a192f;
  color: #64ffda;
  padding: 2rem 0 1rem 0;
  box-shadow: 0 -2px 16px rgba(0,0,0,0.04);
  width: 100%;
  margin-top: 3rem;
  position: static;
}
.footer-content {
  max-width: 900px;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.footer-links {
  display: flex;
  gap: 2.5rem;
  margin-bottom: 1rem;
  flex-wrap: wrap;
  justify-content: center;
}
.footer-link {
  display: flex;
  flex-direction: column;
  align-items: center;
  color: #64ffda;
  text-decoration: none;
  font-size: 1rem;
  font-weight: 500;
  transition: color 0.2s;
}
.footer-link:hover {
  color: #fff;
}
.footer-link svg {
  margin-bottom: 0.3rem;
  transition: stroke 0.2s;
}
.footer-link:hover svg {
  stroke: #fff;
}
.footer-copyright {
  color: #8892b0;
  font-size: 0.95rem;
  margin-top: 0.5rem;
}

@media (max-width: 900px) {
  .footer-links {
    flex-direction: column;
    align-items: center;
    gap: 1.2rem;
    width: 100%;
  }
  .main-footer {
    width: 100%;
    box-sizing: border-box;
    margin-left: 0;
  }
}
</style> 