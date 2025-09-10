<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Adnan - Full Stack Developer</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;500;700&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            background-color: #0d1117;
            color: #ffffff;
            font-family: 'Orbitron', sans-serif;
            line-height: 1.6;
            padding: 20px;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .container {
            background: linear-gradient(135deg, #0d1117 0%, #161b22 100%);
            border-radius: 15px;
            padding: 30px;
            box-shadow: 0 0 30px rgba(0, 255, 221, 0.2), 0 0 60px rgba(255, 0, 255, 0.1);
            border: 1px solid #30363d;
        }
        
        header {
            text-align: center;
            margin-bottom: 40px;
            padding: 20px;
        }
        
        h1 {
            font-size: 2.5rem;
            margin: 20px 0;
            color: #00FFDD;
            text-shadow: 0 0 10px #00FFDD, 0 0 20px #FF00FF;
        }
        
        h2 {
            font-size: 1.8rem;
            margin: 30px 0 20px;
            color: #00FFDD;
            text-shadow: 0 0 5px #00FFDD;
            padding-bottom: 10px;
            border-bottom: 2px solid #FF00FF;
        }
        
        h3 {
            font-size: 1.4rem;
            margin: 20px 0 15px;
            color: #FF00FF;
        }
        
        p {
            margin: 15px 0;
            color: #ffffff;
        }
        
        .badges {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 10px;
            margin: 20px 0;
        }
        
        .badge {
            padding: 8px 15px;
            border-radius: 5px;
            font-size: 0.9rem;
            font-weight: bold;
            text-decoration: none;
            display: inline-block;
            transition: transform 0.3s, box-shadow 0.3s;
            color: #ffffff;
        }
        
        .badge:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0, 255, 221, 0.4);
        }
        
        .divider {
            height: 3px;
            background: linear-gradient(90deg, #00FFDD, #FF00FF);
            margin: 40px 0;
            border-radius: 3px;
        }
        
        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
            margin: 30px 0;
        }
        
        .tech-category {
            background: rgba(22, 27, 34, 0.8);
            padding: 20px;
            border-radius: 10px;
            border: 1px solid #30363d;
            box-shadow: 0 0 15px rgba(0, 255, 221, 0.1);
        }
        
        .tech-items {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 15px;
        }
        
        .tech-item {
            background: rgba(0, 255, 221, 0.1);
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            color: #ffffff;
            border: 1px solid rgba(0, 255, 221, 0.3);
        }
        
        .stats {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
            margin: 30px 0;
        }
        
        .stat-item {
            flex: 1;
            min-width: 280px;
            background: rgba(22, 27, 34, 0.8);
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            border: 1px solid #30363d;
            box-shadow: 0 0 15px rgba(255, 0, 255, 0.1);
        }
        
        .projects {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            margin: 30px 0;
        }
        
        .project {
            background: rgba(22, 27, 34, 0.8);
            padding: 20px;
            border-radius: 10px;
            border: 1px solid #30363d;
            box-shadow: 0 0 15px rgba(0, 255, 221, 0.1);
            transition: transform 0.3s;
        }
        
        .project:hover {
            transform: translateY(-5px);
            box-shadow: 0 0 20px rgba(255, 0, 255, 0.2);
        }
        
        .project-links {
            display: flex;
            gap: 15px;
            margin-top: 15px;
        }
        
        .project-link {
            padding: 8px 15px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s;
            color: #ffffff;
        }
        
        .repo-link {
            background: rgba(0, 255, 221, 0.2);
            border: 1px solid #00FFDD;
        }
        
        .demo-link {
            background: rgba(255, 0, 255, 0.2);
            border: 1px solid #FF00FF;
        }
        
        .project-link:hover {
            opacity: 0.8;
            transform: scale(1.05);
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 15px;
            margin: 30px 0;
        }
        
        .social-link {
            padding: 10px 20px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            display: flex;
            align-items: center;
            gap: 8px;
            transition: all 0.3s;
            color: #ffffff;
        }
        
        .quote {
            text-align: center;
            font-style: italic;
            margin: 40px 0;
            padding: 20px;
            border-radius: 10px;
            background: rgba(22, 27, 34, 0.8);
            border: 1px solid #30363d;
            box-shadow: 0 0 15px rgba(0, 255, 221, 0.1);
            color: #ffffff;
        }
        
        .glow-text {
            text-shadow: 0 0 10px #00FFDD, 0 0 20px #FF00FF;
        }
        
        @media (max-width: 768px) {
            .tech-grid {
                grid-template-columns: 1fr;
            }
            
            .stats {
                flex-direction: column;
            }
            
            .projects {
                grid-template-columns: 1fr;
            }
            
            h1 {
                font-size: 2rem;
            }
            
            h2 {
                font-size: 1.5rem;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>👋 Assalamualaikum! I'm Adnan</h1>
            <p class="glow-text">A Passionate Full-Stack Developer from Bangladesh</p>
            
            <div class="badges">
                <a href="https://github.com/Adnan123456a?tab=followers" class="badge" style="background: #1A1A1A; border: 1px solid #00FFDD;">
                    Followers: 100+
                </a>
                <a href="https://github.com/Adnan123456a" class="badge" style="background: #1A1A1A; border: 1px solid #FF00FF;">
                    Stars: 50+
                </a>
                <a href="https://visitor-badge.laobi.icu/badge?page_id=adnan123456a.adnan123456a" class="badge" style="background: #1A1A1A; border: 1px solid #00FFDD;">
                    Visitors: 500+
                </a>
            </div>
        </header>
        
        <div class="divider"></div>
        
        <section>
            <h2>🌌 Tech Stack</h2>
            
            <div class="tech-grid">
                <div class="tech-category">
                    <h3>🚀 Languages</h3>
                    <div class="tech-items">
                        <span class="tech-item">JavaScript</span>
                        <span class="tech-item">TypeScript</span>
                        <span class="tech-item">Python</span>
                        <span class="tech-item">C</span>
                        <span class="tech-item">Bash</span>
                        <span class="tech-item">HTML5</span>
                        <span class="tech-item">CSS3</span>
                    </div>
                </div>
                
                <div class="tech-category">
                    <h3>⚡ Frontend</h3>
                    <div class="tech-items">
                        <span class="tech-item">React</span>
                        <span class="tech-item">Next.js</span>
                        <span class="tech-item">Tailwind CSS</span>
                        <span class="tech-item">Bootstrap</span>
                    </div>
                </div>
                
                <div class="tech-category">
                    <h3>🔥 Backend</h3>
                    <div class="tech-items">
                        <span class="tech-item">Node.js</span>
                        <span class="tech-item">Express.js</span>
                        <span class="tech-item">NestJS</span>
                        <span class="tech-item">FastAPI</span>
                    </div>
                </div>
                
                <div class="tech-category">
                    <h3>🗄️ Databases</h3>
                    <div class="tech-items">
                        <span class="tech-item">MongoDB</span>
                        <span class="tech-item">MySQL</span>
                        <span class="tech-item">PostgreSQL</span>
                        <span class="tech-item">Redis</span>
                    </div>
                </div>
                
                <div class="tech-category">
                    <h3>🛠️ Tools & Tech</h3>
                    <div class="tech-items">
                        <span class="tech-item">Docker</span>
                        <span class="tech-item">NGINX</span>
                        <span class="tech-item">PM2</span>
                        <span class="tech-item">Postman</span>
                        <span class="tech-item">JWT</span>
                    </div>
                </div>
                
                <div class="tech-category">
                    <h3>☁️ DevOps & Cloud</h3>
                    <div class="tech-items">
                        <span class="tech-item">GitHub</span>
                        <span class="tech-item">GitLab</span>
                        <span class="tech-item">Render</span>
                        <span class="tech-item">Netlify</span>
                        <span class="tech-item">Vercel</span>
                        <span class="tech-item">Git</span>
                    </div>
                </div>
            </div>
        </section>
        
        <div class="divider"></div>
        
        <section>
            <h2>📊 GitHub Stats</h2>
            
            <div class="stats">
                <div class="stat-item">
                    <h3>GitHub Stats</h3>
                    <p>Repositories: 20+</p>
                    <p>Contributions: 500+</p>
                    <p>Commits: 1000+</p>
                </div>
                
                <div class="stat-item">
                    <h3>Streak Stats</h3>
                    <p>Current Streak: 15 days</p>
                    <p>Longest Streak: 60 days</p>
                    <p>Total Contributions: 800+</p>
                </div>
                
                <div class="stat-item">
                    <h3>Top Languages</h3>
                    <p>JavaScript: 45%</p>
                    <p>Python: 25%</p>
                    <p>HTML/CSS: 15%</p>
                    <p>Others: 15%</p>
                </div>
            </div>
        </section>
        
        <div class="divider"></div>
        
        <section>
            <h2>🚀 Featured Projects</h2>
            
            <div class="projects">
                <div class="project">
                    <h3>AniPub - Anime Publishing Platform</h3>
                    <p>A full-stack anime publishing platform with user authentication, content management, and responsive design.</p>
                    <div class="project-links">
                        <a href="https://github.com/AnimePub" class="project-link repo-link">Repository</a>
                        <a href="https://anipub.adnandluffy.com/" class="project-link demo-link">Live Demo</a>
                    </div>
                </div>
                
                <div class="project">
                    <h3>MDA Server</h3>
                    <p>A powerful server implementation with RESTful APIs, database integration, and authentication systems.</p>
                    <div class="project-links">
                        <a href="https://github.com/AdnanDLuffy/MDA-Server" class="project-link repo-link">Repository</a>
                    </div>
                </div>
                
                <div class="project">
                    <h3>SMTPulse - Email Service</h3>
                    <p>An email service solution with SMTP integration, template management, and analytics.</p>
                    <div class="project-links">
                        <a href="https://github.com/Adnan-D-Luffy/smtpulse" class="project-link repo-link">Repository</a>
                    </div>
                </div>
            </div>
        </section>
        
        <div class="divider"></div>
        
        <section>
            <h2>📡 Connect With Me</h2>
            
            <div class="social-links">
                <a href="https://www.facebook.com/WallaHabibi.Adnan" class="social-link" style="background: #1877F2;">
                    Facebook
                </a>
                <a href="https://www.instagram.com/adnand.luffy" class="social-link" style="background: #E4405F;">
                    Instagram
                </a>
                <a href="https://github.com/adnan123456a" class="social-link" style="background: #6e5494;">
                    GitHub
                </a>
                <a href="mailto:youremail@example.com" class="social-link" style="background: #EA4335;">
                    Email
                </a>
            </div>
        </section>
        
        <div class="divider"></div>
        
        <div class="quote">
            <p class="glow-text">💡 "Code the future, one commit at a time!"</p>
        </div>
    </div>

    <script>
        // Simple animation for tech items
        document.addEventListener('DOMContentLoaded', function() {
            const techItems = document.querySelectorAll('.tech-item');
            techItems.forEach((item, index) => {
                item.style.animationDelay = `${index * 0.1}s`;
                item.classList.add('fade-in');
            });
            
            // Add animation for project cards
            const projects = document.querySelectorAll('.project');
            projects.forEach((project, index) => {
                project.style.animationDelay = `${index * 0.2}s`;
                project.classList.add('fade-in-up');
            });
        });
    </script>
</body>
</html>
