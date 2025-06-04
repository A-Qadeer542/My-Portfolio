<script lang="ts">
  import ProjectCard from '$lib/components/ProjectCard.svelte';
  type Project = {
    imageUrl: string;
    title: string;
    description: string;
    link: string | undefined;
  };
  const featuredProjects: Project[] = [

    {
        imageUrl: '/matrix.jpg',
        title: 'Matrix™ MK II+',
        description: 'The Matrix is a stand-alone fibre optic multiplexer and control solution, providing an interactive touch-screen UI for a large array of sensors and equipment to any remotely operated system.',
        link: 'https://www.innova.no/product/matrix-multiplexer/matrix-mk-ii/'
    },

    {
      imageUrl: '/icebox.png',
      title: 'Icebox Plugin Development',
      description: 'Organization of maintenance plug-ins for SLB oil and gas applications, Petrel, Techlog and Studio.',
      link: 'https://commerce.slb.com/slb/en/USD/Ocean-Store/Plug-ins/c/plugin'
    },

    {
      imageUrl: '/therma.jpg',
      title: 'Therma Plugin',
      description: 'Distributed temperature and acoustic sensing (DAS) analysis software for 2D/3D visualization and wellbore temperature profiles.',
      link: 'https://www.slb.com/products-and-services/innovating-in-oil-and-gas/completions/well-completions/permanent-monitoring/distributed-permanent-measurement-systems/distributed-permanent-measurement-system-accessories/therma-software'
    },

    {
      imageUrl: '/survey-merge.jpg',
      title: 'Survey Merge',
      description: 'Merges several 3D cubes of different survey/orientation into a single output cube defined by the user.',
      link: 'https://commerce.slb.com/slb/en/USD/oceanProduct/Survey%20Merge'
    },

    {
      imageUrl: '/wellview.jpg',
      title: 'WellView – MasterView Connector',
      description: 'The WellView/MasterView Connector connects Petrel and Studio Manager end-users to the WellView/MasterView database.',
      link: 'https://commerce.slb.com/slb/en/USD/oceanProduct/WellView%20-%20MasterView%20Connector'
    },

    {
      imageUrl: '/innovation-factori.png',
      title: 'Innovation Factori',
      description: 'Accelerating AI adoption for the energy industry where oil and gas meet Machine Learning driven technologies.',
      link: 'https://www.software.slb.com/ai/innovation-factori?trk=public_post_comment-text'
    },

    {
        imageUrl: '/ora2petrel.png',
        title: 'Ora2Petrel',
        description: 'This plug-in allows to load various data from corporate database into Petrel. It is enabled in workflow manager. This functionality combined with local model update and automated history match helps to keep models up-to-date.',
        link: 'https://commerce.slb.com/slb/en/USD/oceanProduct/Ora2Petrel'
    },
    
    {
        imageUrl: '/tkhelse.jpg',
        title: 'Petrel',
        description: 'Digital Invoicing System to send reminders to patients and remittances to doctors.',
        link: 'http://tkhelse.no/'
    }
  ];
</script>

<section class="home-hero-section">
  <img src="/my-icon.jpg" alt="Abdul Qadeer" class="profile-img" />
  <h1>Abdul Qadeer</h1>
  <h2>Software Developer</h2>
  <p>
    I am a software developer with strong expertise in developing desktop and full-stack web applications, and deploying cloud-based solutions. I deliver innovative technologies across various platforms.
  </p>
</section>

<section class="home-featured-projects-section">
  <h2>Featured Projects</h2>
  <div class="home-projects-grid">
    {#each featuredProjects as project}
      <ProjectCard {...project} />
    {/each}
  </div>
</section>

<style>
:global(html, body) {
  overflow-x: hidden;
}
.home-hero-section, .home-featured-projects-section {
  box-sizing: border-box;
}
.home-hero-section {
  text-align: center;
  padding: 3rem 1rem 2rem 1rem;
}
.profile-img {
  width: 120px;
  height: 120px;
  border-radius: 50%;
  object-fit: cover;
  margin-bottom: 1rem;
  border: 4px solid #64ffda;
}
.home-hero-section h1 {
  margin: 0.5rem 0 0.2rem 0;
  font-size: 2.5rem;
  color: #0a192f;
}
.home-hero-section h2 {
  margin: 0 0 1rem 0;
  color: #8892b0;
  font-size: 1.3rem;
}
.home-hero-section p {
  color: #333;
  max-width: 600px;
  margin: 0 auto;
}
.home-featured-projects-section {
  padding: 2rem 1rem;
  background: #f5f7fa;
}
.home-featured-projects-section h2 {
  text-align: center;
  color: #0a192f;
  margin-bottom: 2rem;
}
.home-projects-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 2rem;
  justify-content: center;
}
</style> 