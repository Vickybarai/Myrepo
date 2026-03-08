<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vicky Barai | DevOps Portfolio</title>
    <style>
        /* ================= CSS VARIABLES & RESET ================= */
        :root {
            --bg-color: #0d1117;        /* GitHub Dark Dimmed background */
            --card-bg: #161b22;         /* Slightly lighter for cards */
            --text-main: #e6edf3;       /* Main text */
            --text-muted: #8b949e;      /* Secondary text */
            --accent-color: #2ea44f;    /* The Green from your request */
            --border-color: #30363d;    /* Subtle borders */
            --shadow: 0 4px 12px rgba(0, 0, 0, 0.5);
            --font-main: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-main);
            font-family: var(--font-main);
            line-height: 1.6;
            padding-bottom: 50px;
        }

        /* ================= LAYOUT UTILITIES ================= */
        .container {
            max-width: 1000px;
            margin: 0 auto;
            padding: 20px;
        }

        .section-card {
            background-color: var(--card-bg);
            border: 1px solid var(--border-color);
            border-radius: 12px;
            padding: 30px;
            margin-bottom: 30px;
            box-shadow: var(--shadow);
        }

        h2 {
            color: var(--accent-color);
            font-size: 1.8em;
            margin-bottom: 20px;
            border-bottom: 1px solid var(--border-color);
            padding-bottom: 10px;
        }

        h3 {
            color: var(--text-main);
            margin-top: 15px;
            margin-bottom: 10px;
            font-size: 1.3em;
        }

        p {
            color: var(--text-muted);
            margin-bottom: 15px;
        }

        ul {
            list-style-position: inside;
            color: var(--text-muted);
        }

        li {
            margin-bottom: 8px;
        }

        /* Images are responsive by default */
        img {
            max-width: 100%;
            height: auto;
            display: block;
        }

        /* ================= HEADER ================= */
        header {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            margin-bottom: 40px;
            margin-top: 20px;
        }

        .header-content {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 30px;
            flex-wrap: wrap; /* Allows stacking on mobile */
        }

        .profile-img-wrapper {
            border-radius: 50%;
            border: 4px solid var(--accent-color);
            box-shadow: 0 8px 22px rgba(0,0,0,0.35);
            overflow: hidden;
            width: 250px; /* Constrain width for better layout control */
            height: 250px;
            flex-shrink: 0; /* Prevents squishing */
        }

        .profile-img-wrapper img {
            width: 100%;
            height: 100%;
            object-fit: cover; /* Ensures image fills circle without distortion */
        }

        .header-text h1 {
            font-size: 2.5em;
            margin: 0;
        }

        .header-text .role {
            font-size: 1.2em;
            color: var(--text-muted);
            margin-top: 8px;
        }

        .highlight {
            color: var(--accent-color);
        }

        /* ================= SECTIONS SPECIFICS ================= */
        
        /* DevOps Cycle */
        .devops-cycle {
            text-align: center;
            margin: 20px 0;
            font-weight: bold;
            color: var(--text-main);
            letter-spacing: 1px;
            font-size: 0.9em;
        }

        /* Skills Grid */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
        }

        /* Projects List */
        .project-item {
            margin-bottom: 20px;
            padding-bottom: 20px;
            border-bottom: 1px solid var(--border-color);
        }
        .project-item:last-child {
            border-bottom: none;
            padding-bottom: 0;
            margin-bottom: 0;
        }

        /* Badges Container */
        .badges-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 10px;
            margin: 20px 0;
        }
        
        /* GitHub Stats */
        .stats-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
            margin-top: 20px;
        }
        
        .stats-container img {
            border-radius: 8px;
        }

        /* Footer Quote */
        .footer-quote {
            text-align: center;
            font-style: italic;
            color: var(--accent-color);
            margin-top: 30px;
            font-size: 1.1em;
        }

        /* ================= RESPONSIVE ADJUSTMENTS ================= */
        @media (max-width: 768px) {
            header {
                text-align: center;
            }
            .header-content {
                flex-direction: column;
                gap: 20px;
            }
            .header-text h1 {
                font-size: 2em;
            }
            .profile-img-wrapper {
                width: 200px;
                height: 200px;
            }
            .stats-container {
                flex-direction: column;
                align-items: center;
            }
        }
    </style>
</head>
<body>

<div class="container">

    <!-- ================= HEADER ================= -->
    <header>
        <div class="header-content">
            <!-- Profile Image -->
            <div class="profile-img-wrapper">
                <img src="https://media.giphy.com/media/qgQUggAC3Pfv687qPC/giphy.gif"
                     alt="DevOps Profile"/>
            </div>
            
            <!-- Name + Role -->
            <div class="header-text">
                <h1>Hi 👋, I'm <span class="highlight">Vicky Barai</span></h1>
                <p class="role">Aspiring DevOps | MCA Final Year Student</p>
            </div>
        </div>
    </header>

    <!-- ================= ABOUT ================= -->
    <section class="section-card">
        <h2>🚀 About Me</h2>
        <p>
            I am a <b>Vicky Barai</b> and an <b>early-career DevOps </b> actively building
            hands-on experience in Linux, AWS, CI/CD pipelines, containerization, and infrastructure automation.
        </p>
        <p>
            My learning focuses on deploying applications on cloud infrastructure,
            automating build and deployment workflows,
            and managing infrastructure using code.
            I am continuously strengthening my skills through real-world DevOps projects.
        </p>
        <p>
            I believe in <b>automation over repetition</b> and <b>learning by doing</b>.
        </p>
    </section>

    <!-- ================= DEVOPS LIFECYCLE ================= -->
    <section class="section-card" style="text-align: center;">
        <img src="https://stemettes.org/zine/wp-content/uploads/sites/3/2021/08/DEVOPS.gif"
             alt="DevOps Lifecycle"
             style="border-radius:12px; box-shadow:0 6px 20px rgba(0,0,0,0.25); margin: 0 auto 15px auto;" />
        
        <div class="devops-cycle">
            Plan → Code → Build → Test → Release → Deploy → Operate → Monitor
        </div>
    </section>

    <!-- ================= SKILLS ================= -->
    <section class="section-card">
        <h2>🛠️ Skills & Tools</h2>
        <div class="skills-grid">
            <ul>
                <li><b>Operating System:</b> Linux (basic administration, permissions, services)</li>
                <li><b>Cloud:</b> AWS (EC2, S3, IAM, RDS, VPC, CloudWatch)</li>
                <li><b>Version Control:</b> Git, GitHub</li>
                <li><b>CI/CD:</b> Jenkins, GitHub Actions (basic pipelines)</li>
            </ul>
            <ul>
                <li><b>Containers:</b> Docker, Docker Compose, Kubernetes (fundamentals)</li>
                <li><b>Infrastructure as Code:</b> Terraform (basic modules & provisioning)</li>
                <li><b>Scripting:</b> Shell scripting, Python (basics)</li>
            </ul>
        </div>
    </section>

    <!-- ================= PROJECTS ================= -->
    <section class="section-card">
        <h2>🏗️ Projects</h2>
        
        <div class="project-item">
            <h3>🐳 Containerized Web Application</h3>
            <ul>
                <li>Built and containerized a web application using Docker</li>
                <li>Worked with Docker images, containers, volumes, and networks</li>
                <li>Deployed containers on Linux-based cloud instances</li>
            </ul>
        </div>

        <div class="project-item">
            <h3>🔄 CI/CD Pipeline Automation</h3>
            <ul>
                <li>Created basic CI/CD pipelines using Jenkins</li>
                <li>Integrated GitHub repositories with Jenkins jobs</li>
                <li>Automated build and deployment workflows</li>
            </ul>
        </div>

        <div class="project-item">
            <h3>☸️ Kubernetes Deployment (Learning Project)</h3>
            <ul>
                <li>Deployed containerized applications using Kubernetes</li>
                <li>Worked with Pods, Deployments, Services, and basic scaling</li>
                <li>Explored ConfigMaps and Secrets</li>
            </ul>
        </div>

        <div class="project-item">
            <h3>🏗️ Infrastructure Automation with Terraform</h3>
            <ul>
                <li>Provisioned AWS resources using Terraform</li>
                <li>Created EC2 instances and supporting infrastructure</li>
                <li>Worked with Terraform state and reusable configurations</li>
            </ul>
        </div>
    </section>

    <!-- ================= SKILLS BADGES & TOOLS ================= -->
    <section class="section-card">
        <h2 style="text-align: center; border: none;">🚀 DevOps Skills & Tools</h2>
        
        <div class="badges-container">
            <!-- OS -->
            <img src="https://img.shields.io/badge/Linux-000000?style=for-the-badge&logo=linux&logoColor=white" alt="Linux"/>
            <!-- Cloud -->
            <img src="https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="AWS"/>
            <img src="https://img.shields.io/badge/Amazon%20EC2-FF9900?style=for-the-badge&logo=amazon-ec2&logoColor=white" alt="EC2"/>
            <img src="https://img.shields.io/badge/Amazon%20S3-569A31?style=for-the-badge&logo=amazon-s3&logoColor=white" alt="S3"/>
            <img src="https://img.shields.io/badge/IAM-DD344C?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="IAM"/>
            <img src="https://img.shields.io/badge/Amazon%20RDS-527FFF?style=for-the-badge&logo=amazon-rds&logoColor=white" alt="RDS"/>
            <img src="https://img.shields.io/badge/Amazon%20VPC-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="VPC"/>
            <img src="https://img.shields.io/badge/CloudWatch-FF4F8B?style=for-the-badge&logo=amazon-cloudwatch&logoColor=white" alt="CloudWatch"/>
            <!-- DevOps / CI-CD -->
            <img src="https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white" alt="Jenkins"/>
            <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white" alt="GitHub Actions"/>
            <!-- Containers -->
            <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker"/>
            <img src="https://img.shields.io/badge/Docker%20Compose-1488C6?style=for-the-badge&logo=docker&logoColor=white" alt="Docker Compose"/>
            <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" alt="Kubernetes"/>
            <!-- IaC -->
            <img src="https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white" alt="Terraform"/>
            <!-- Version Control -->
            <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git"/>
            <img src="https://img.shields.io/badge/GitHub-121011?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
            <!-- Scripting -->
            <img src="https://img.shields.io/badge/Shell%20Scripting-4EAA25?style=for-the-badge&logo=gnu-bash&logoColor=white" alt="Shell"/>
            <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
        </div>

        <div style="text-align: center; margin-top: 30px;">
            <img src="https://media.giphy.com/media/LMt9638dO8dftAjtco/giphy.gif"
                 alt="DevOps Automation"
                 width="200" height="200"
                 style="border-radius:14px; box-shadow:0 6px 22px rgba(0,0,0,0.3); display: inline-block;" />
        </div>
    </section>

    <!-- ================= GITHUB STATS ================= -->
    <section class="section-card">
        <h2>📊 GitHub Stats</h2>
        <div class="stats-container">
          #  <img src="https://github-readme-stats.vercel.app/api?username=Vickybarai&theme=dark&hide_border=true&include_all_commits=true&count_private=false" alt="Stats"/>
            <img src="https://nirzak-streak-stats.vercel.app/?user=Vickybarai&theme=dark&hide_border=true" alt="Streak"/>
           # <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Vickybarai&theme=dark&hide_border=true&include_all_commits=true&count_private=false&layout=compact" alt="Top Langs"/>
            <img src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=radical" alt="Quote"/>
        </div>
        
        <!-- Footer Image -->
        <div style="text-align: center; margin-top: 30px;">
             <img src="https://stemettes.org/zine/wp-content/uploads/sites/3/2021/08/6oFTUDQ-1.gif"
                 alt="DevOps Automation"
                 width="420"
                 style="border-radius:14px; box-shadow:0 6px 22px rgba(0,0,0,0.3); max-width: 100%; margin: 0 auto;" />
        </div>
    </section>

    <!-- ================= FOOTER ================= -->
    <div class="footer-quote">
        <p>Learning • Building • Automating • Improving</p>
    </div>

</div>

</body>
</html>
