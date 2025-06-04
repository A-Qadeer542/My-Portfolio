<script lang="ts">
// No logic needed for now
</script>

<section class="skills-section">
  <h1 class="skills-title">Skills</h1>
  <div class="skills-grid">
    <div class="skill-card">
      <div class="skill-icon">💻</div>
      <h2>Programming Languages</h2>
      <ul>
        <li>C#</li>
        <li>JavaScript</li>
        <li>C++</li>
        <li>Python</li>
        <li>TypeScript</li>
        <li>PL/SQL</li>
        <li>SQL</li>
      </ul>
    </div>
    <div class="skill-card">
        <div class="skill-icon">🌐</div>
        <h2>Web Development</h2>
        <ul>
          <li>Svelte</li>
          <li>React.js</li>
          <li>HTML</li>
          <li>CSS</li>
          <li>Bootstrap 4</li>
          <li>JQuery</li>
          <li>AngularJS</li>
          <li>PHP</li>
        </ul>
      </div>
    <div class="skill-card">
      <div class="skill-icon">📚</div>
      <h2>Framework and Libraries</h2>
      <ul>
        <li>.NET Framework</li>
        <li>.NET Core</li>
        <li>Laravel</li>
        <li>Model-View-ViewModel(MVVM)</li>
        <li>Model-View-Controller(MVC)</li>
        <li>Windows Presentation Foundation (WPF)</li>
        <li>WinForms</li>
        <li>QT</li>
      </ul>
    </div>
    <div class="skill-card">
      <div class="skill-icon">🗄️</div>
      <h2>Databases</h2>
      <ul>
        <li>Oracle Database</li>
        <li>MySQL</li>
      </ul>
    </div>
    <div class="skill-card">
      <div class="skill-icon">☁️</div>
      <h2>DevOps and Cloud Platforms</h2>
      <ul>
        <li>AWS</li>
        <li>Azure DevOps</li>
        <li>EC2 Linux Server Deployment and Management</li>
      </ul>
    </div>
    <div class="skill-card">
      <div class="skill-icon">⚙️</div>
      <h2>Tools and Automation</h2>
      <ul>
        <li>Git</li>
        <li>Bitbucket</li>
        <li>Team Foundation Server</li>
        <li>PowerShell</li>
        <li>CI/CD Pipelines</li>
      </ul>
    </div>
    <div class="skill-card">
      <div class="skill-icon">🧪</div>
      <h2>Testing</h2>
      <ul>
        <li>NUnit</li>
        <li>Unit testing</li>
      </ul>
    </div>
    <div class="skill-card">
      <div class="skill-icon">📈</div>
      <h2>Software Development Methodologies</h2>
      <ul>
        <li>Agile</li>
        <li>Scum</li>
        <li>Ghannt Charts</li>
      </ul>
    </div>
    <div class="skill-card">
      <div class="skill-icon">✨</div>
      <h2>Other Skills</h2>
      <ul>
        <li>RaspBerry Pi CM4</li>
        <li>Debugging</li>
        <li>Software Documentation</li>
        <li>Communication</li>
        <li>Team Leadership</li>
        <li>Management</li>
      </ul>
    </div>
  </div>
</section>

<style>
.skills-section {
  padding: 3rem 1rem 2rem 1rem;
  max-width: 1200px;
  margin: 0 auto;
}
.skills-title {
  text-align: center;
  font-size: 2.3rem;
  color: #0a192f;
  margin-bottom: 2.5rem;
  font-weight: bold;
}
.skills-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 2.5rem;
}
.skill-card {
  background: #fff;
  border-radius: 16px;
  box-shadow: 0 2px 12px rgba(0,0,0,0.07);
  padding: 2rem 1.5rem 1.5rem 1.5rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  transition: box-shadow 0.2s, transform 0.2s;
  cursor: pointer;
}
.skill-card:hover {
  box-shadow: 0 8px 24px rgba(100,255,218,0.18), 0 2px 8px rgba(0,0,0,0.10);
  transform: scale(1.04) translateY(-4px);
}
.skill-icon {
  font-size: 2.2rem;
  margin-bottom: 1rem;
}
.skill-card h2 {
  color: #0a192f;
  font-size: 1.3rem;
  margin-bottom: 1rem;
  text-align: center;
}
.skill-card ul {
  list-style: disc inside;
  padding-left: 0.5rem;
  margin: 0;
  text-align: left;
  list-style-position: inside;
  word-break: break-word;
}
.skill-card li {
  color: #333;
  font-size: 1.08rem;
  margin-bottom: 0.5rem;
  line-height: 1.5;
  padding-left: 0.2rem;
}
@media (max-width: 700px) {
  .skills-grid {
    grid-template-columns: 1fr;
  }
  .skills-section {
    padding: 2rem 0.5rem 1rem 0.5rem;
  }
}
</style> 