<script lang="ts">
  export let imageUrl: string;
  export let title: string;
  export let description: string;
  export let link: string | undefined;
</script>

{#if link}
  <a href={link} target="_blank" rel="noopener noreferrer" class="project-card-link">
    <div class="project-card">
      <img src={imageUrl} alt={title} class="project-card-image" />
      <h3 class="project-card-title">{title}</h3>
      <p class="project-card-description">{description}</p>
    </div>
  </a>
{:else}
  <div class="project-card">
    <img src={imageUrl} alt={title} class="project-card-image" />
    <h3 class="project-card-title">{title}</h3>
    <p class="project-card-description">{description}</p>
  </div>
{/if}

<style>
.project-card {
  background: #fff;
  border-radius: 12px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.07);
  padding: 1.5rem;
  max-width: 370px;
  min-width: 320px;
  min-height: 360px;
  max-height: 360px;
  text-align: left;
  transition: box-shadow 0.2s, transform 0.2s;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  cursor: pointer;
}
@media (max-width: 600px) {
  .project-card {
    min-width: 0;
    max-width: 100%;
    min-height: 380px;
    max-height: 380px;
    padding: 1rem;
  }
}
.project-card:hover {
  transform: scale(1.04) translateY(-4px);
}
.project-card-image {
  width: 100%;
  height: 200px;
  object-fit: cover;
  border-radius: 8px;
  margin-bottom: 1rem;
}
.project-card-title {
  margin: 0.5rem 0 0.2rem 0;
  color: #0a192f;
  font-size: 1.25rem;
  font-weight: bold;
}
.project-card-description {
  color: #555;
  font-size: 1rem;
  flex: 1 1 auto;
  overflow: hidden;
  text-overflow: ellipsis;
}
.project-card-link {
  text-decoration: none;
  color: inherit;
  display: block;
}
</style> 