<script lang="ts">
// No logic needed for now
</script>

<section class="contact-section">
  <h1 class="contact-title">Contact Information</h1>
  <div class="contact-grid">
    <div class="contact-info">
      <div class="contact-item">
        <svg width="22" height="22" fill="none" stroke="#64ffda" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M22 16.92v3a2 2 0 0 1-2.18 2A19.72 19.72 0 0 1 3.08 5.18 2 2 0 0 1 5 3h3a2 2 0 0 1 2 1.72c.13.81.36 1.6.7 2.34a2 2 0 0 1-.45 2.11l-1.27 1.27a16 16 0 0 0 6.29 6.29l1.27-1.27a2 2 0 0 1 2.11-.45c.74.34 1.53.57 2.34.7A2 2 0 0 1 21 16.92z"/></svg>
        <span>+47 967 15 695</span>
      </div>
      <div class="contact-item">
        <svg width="22" height="22" fill="none" stroke="#64ffda" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="M22 6 12 13 2 6"/></svg>
        <a href="mailto:1124abdul@gmail.com">1124abdul@gmail.com</a>
      </div>
      <div class="contact-item">
        <svg width="22" height="22" fill="none" stroke="#64ffda" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M17.657 16.657L13.414 12.414a4 4 0 1 0-1.414 1.414l4.243 4.243a1 1 0 0 0 1.414-1.414z"/><circle cx="11" cy="11" r="8"/></svg>
        <span>Madlamarkveien 6, 4041 Stavanger</span>
      </div>
    </div>
    <div class="contact-map">
      <iframe
        src="https://www.openstreetmap.org/export/embed.html?bbox=5.6935%2C58.9645%2C5.6955%2C58.9665&amp;layer=mapnik&amp;marker=58.9655%2C5.6945"
        style="border:1px solid #ccc; border-radius: 10px; width:100%; height:250px;"
        allowfullscreen
        loading="lazy"
        referrerpolicy="no-referrer-when-downgrade"
        title="Map to Madlamarkveien 6"
      ></iframe>
    </div>
  </div>
</section>

<style>
.contact-section {
  padding: 2rem 1rem 1rem 1rem;
  max-width: 900px;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
  min-height: 60vh;
}
.contact-title {
  text-align: center;
  font-size: 2.2rem;
  color: #0a192f;
  margin-bottom: 2rem;
  font-weight: bold;
}
.contact-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 2.5rem;
  width: 100%;
  justify-content: center;
}
.contact-info {
  display: flex;
  flex-direction: column;
  gap: 1.2rem;
  min-width: 220px;
  justify-content: center;
}
.contact-item {
  display: flex;
  align-items: center;
  gap: 0.7rem;
  font-size: 1.1rem;
  color: #0a192f;
}
.contact-item a {
  color: #64ffda;
  text-decoration: none;
  transition: color 0.2s;
}
.contact-item a:hover {
  color: #0a192f;
  text-decoration: underline;
}
.contact-map {
  min-width: 320px;
  max-width: 500px;
  flex: 1 1 320px;
  display: flex;
  align-items: center;
  justify-content: center;
}
.contact-map iframe {
  width: 100%;
  height: 320px;
  border: 1px solid #ccc;
  border-radius: 10px;
}
@media (max-width: 700px) {
  .contact-grid {
    flex-direction: column;
    align-items: center;
    gap: 1.5rem;
  }
  .contact-section {
    padding: 2rem 0.5rem 1rem 0.5rem;
  }
}
</style> 