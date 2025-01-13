<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>GitHub Home Page Portfolio</title>
  <style>
    :root {
      --background-color: #f9fafb;
      --text-color: #1f2937;
      --card-background-color: #ffffff;
      --card-border-color: #e5e7eb;
      --icon-color: #6b7280;
      --primary-color: #3b82f6;
      --secondary-color: #6574cd;
      --accent-color: #fbbf24;
    }
    [data-theme="dark"] {
      --background-color: #1f2937;
      --text-color: white;
      --card-background-color: #374151;
      --card-border-color: #4b5563;
      --icon-color: #9ca3af;
      --primary-color: #60a5fa;
      --secondary-color: #818cf8;
      --accent-color: #facc15;
    }
    body {
      background-color: var(--background-color);
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 1rem;
      font-family: Arial, sans-serif;
      color: var(--text-color);
      transition: background-color 0.3s, color 0.3s;
    }
    .container {
      width: 100%;
      max-width: 800px;
      margin: 0 auto;
    }
    .section {
      margin-bottom: 2rem;
    }
    .card {
      background-color: var(--card-background-color);
      border: 1px solid var(--card-border-color);
      border-radius: 0.5rem;
      box-shadow: 0 1px 3px rgba(0, 0, 0, 0.1);
      padding: 1.5rem;
      margin-bottom: 1rem;
      transition: box-shadow 0.3s;
    }
    .card:hover {
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    }
    .card-header {
      display: flex;
      align-items: center;
      margin-bottom: 1rem;
    }
    .card-header img {
      width: 6rem;
      height: 6rem;
      border-radius: 50%;
      margin-right: 1rem;
    }
    .card-title {
      font-size: 1.5rem;
      font-weight: bold;
      margin-bottom: 0.5rem;
    }
    .card-description {
      color: var(--icon-color);
      margin-bottom: 1rem;
    }
    .card-content {
      margin-bottom: 1rem;
    }
    .card-content img {
      width: 1.5rem;
      height: 1.5rem;
      margin-right: 0.5rem;
    }
    .card-content a {
      text-decoration: none;
      color: var(--primary-color);
    }
    .card-content a:hover {
      text-decoration: underline;
    }
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 1rem;
    }
    .grid-item {
      background-color: var(--card-background-color);
      border: 1px solid var(--card-border-color);
      border-radius: 0.5rem;
      padding: 1rem;
      display: flex;
      flex-direction: column;
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .grid-item:hover {
      transform: translateY(-5px);
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    }
    .grid-item img {
      width: 1.5rem;
      height: 1.5rem;
      margin-right: 0.5rem;
    }
    .grid-item-title {
      font-size: 1.25rem;
      font-weight: bold;
      margin-bottom: 0.5rem;
    }
    .grid-item-description {
      color: var(--icon-color);
    }
    .icon {
      width: 24px;
      height: 24px;
      margin-right: 8px;
    }
    .color-toggle {
      position: fixed;
      top: 1rem;
      right: 1rem;
      background-color: var(--card-background-color);
      border: 1px solid var(--card-border-color);
      border-radius: 0.5rem;
      padding: 0.5rem 1rem;
      cursor: pointer;
      transition: background-color 0.3s, border-color 0.3s;
    }
    .color-toggle:hover {
      background-color: var(--card-border-color);
    }
    .section-title {
      font-size: 2rem;
      font-weight: bold;
      margin-bottom: 1rem;
      color: #f9fafb;
    }
    .section-description {
    color: white;
      margin-bottom: 1rem;
    }
    .about-me {
    background-color: #13b375;
    color: white;
    border-color: #13b375;
    }
    .projects {
      background-color: var(--accent-color);
      color: white;
      border-color: var(--accent-color);
    }
    .skills {
      background-color: var(--primary-color);
      color: white;
      border-color: var(--primary-color);
    }
    .contact {
      background-color: var(--secondary-color);
      color: white;
      border-color: var(--secondary-color);
    }
  </style>
</head>
<body>
  <div class="container">
    <!-- Color Toggle Button -->
    <button class="color-toggle" onclick="toggleTheme()">Toggle Theme</button>

    <!-- Profile Overview Section -->
    <section class="section">
      <div class="card">
        <div class="card-header">
          <img src="https://github.com/nutlope.png" alt="Profile Picture">
          <div>
            <div class="card-title">John Doe</div>
            <div class="card-description">Software Engineer | Passionate about building scalable web applications.</div>
            <div class="card-content">
              <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/mail.svg" alt="Mail" class="icon">
              johndoe@example.com
            </div>
            <div class="card-content">
              <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linkedin.svg" alt="LinkedIn" class="icon">
              <a href="https://linkedin.com/in/johndoe" target="_blank">LinkedIn</a>
            </div>
            <div class="card-content">
              <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/github.svg" alt="GitHub" class="icon">
              <a href="https://github.com/johndoe" target="_blank">GitHub</a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Description Section -->
    <section class="section">
      <div class="card about-me">
        <div class="section-title">About Me</div>
        <div class="section-description">
          Hi there! I'm John Doe, a software engineer with a passion for building scalable web applications. I enjoy working on projects that challenge me and help me grow as a developer. When I'm not coding, you can find me hiking or experimenting with new technologies.
        </div>
      </div>
    </section>

    <!-- Experience Section -->
    <section class="section">
      <div class="card">
        <div class="section-title">Experience</div>
        <div class="grid">
          <div class="grid-item">
            <div class="grid-item-title">Software Engineer</div>
            <div class="grid-item-description">Tech Company XYZ | 2020 - Present</div>
            <div class="grid-item-description">- Developed and maintained web applications using React and TypeScript.</div>
            <div class="grid-item-description">- Collaborated with cross-functional teams to deliver high-quality software.</div>
          </div>
          <div class="grid-item">
            <div class="grid-item-title">Junior Software Engineer</div>
            <div class="grid-item-description">Tech Company ABC | 2018 - 2020</div>
            <div class="grid-item-description">- Assisted in the development of web applications.</div>
            <div class="grid-item-description">- Participated in code reviews and provided feedback.</div>
          </div>
        </div>
      </div>
    </section>

    <!-- Projects Section -->
    <section class="section">
      <div class="card projects">
        <div class="section-title">Projects</div>
        <div class="grid">
          <div class="grid-item">
            <div class="flex items-center">
              <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/General/play.svg" alt="Play" class="icon">
              <div class="grid-item-title">Project 1</div>
            </div>
            <div class="grid-item-description">A brief description of project 1.</div>
          </div>
          <div class="grid-item">
            <div class="flex items-center">
              <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/General/shield.svg" alt="Shield" class="icon">
              <div class="grid-item-title">Project 2</div>
            </div>
            <div class="grid-item-description">A brief description of project 2.</div>
          </div>
          <div class="grid-item">
            <div class="flex items-center">
              <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/General/clock.svg" alt="Clock" class="icon">
              <div class="grid-item-title">Project 3</div>
            </div>
            <div class="grid-item-description">A brief description of project 3.</div>
          </div>
        </div>
      </div>
    </section>

    <!-- Skills Section -->
    <section class="section">
      <div class="card skills">
        <div class="section-title">Skills</div>
        <div class="grid">
          <div class="grid-item">
            <div class="flex items-center">
              <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="React" class="icon">
              <div class="grid-item-title">React</div>
            </div>
            <div class="grid-item-description">Expert in building interactive UIs with React.</div>
          </div>
          <div class="grid-item">
            <div class="flex items-center">
              <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-original.svg" alt="TypeScript" class="icon">
              <div class="grid-item-title">TypeScript</div>
            </div>
            <div class="grid-item-description">Proficient in using TypeScript for type-safe development.</div>
          </div>
          <div class="grid-item">
            <div class="flex items-center">
              <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/users/users-original.svg" alt="Users" class="icon">
              <div class="grid-item-title">Team Collaboration</div>
            </div>
            <div class="grid-item-description">Experienced in working with teams to deliver projects.</div>
          </div>
        </div>
      </div>
    </section>

    <!-- Contact Section -->
    <section class="section">
      <div class="card contact">
        <div class="section-title">Contact</div>
        <div class="card-content">
          <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/mail.svg" alt="Mail" class="icon">
          <a href="mailto:johndoe@example.com">johndoe@example.com</a>
        </div>
        <div class="card-content">
          <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linkedin.svg" alt="LinkedIn" class="icon">
          <a href="https://linkedin.com/in/johndoe" target="_blank">LinkedIn</a>
        </div>
        <div class="card-content">
          <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/github.svg" alt="GitHub" class="icon">
          <a href="https://github.com/johndoe" target="_blank">GitHub</a>
        </div>
      </div>
    </section>
  </div>

  <script>
    function toggleTheme() {
      const body = document.body;
      body.dataset.theme = body.dataset.theme === 'dark' ? 'light' : 'dark';
    }
  </script>
</body>
</html>
