<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vicky Barai - DevOps Profile</title>
    <style>
        /* ================= GLOBAL VARIABLES & RESET ================= */
        :root {
            --bg-color: #0d1117;       /* GitHub Dark Background */
            --card-bg: #161b22;        /* Slightly lighter for cards */
            --text-main: #c9d1d9;      /* Main text */
            --text-muted: #8b949e;     /* Muted text */
            --accent: #2ea44f;         /* GitHub Green */
            --border: #30363d;         /* Border color */
            --shadow: 0 8px 24px rgba(0,0,0,0.5);
        }

        * { box-sizing: border-box; }

        body {
            background-color: var(--bg-color);
            color: var(--text-main);
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif;
            margin: 0;
            padding: 20px;
            line-height: 1.6;
        }

        /* ================= LAYOUT CONTAINER ================= */
        .container {
            max-width: 900px;
            margin: 0 auto;
            background-color: var(--bg-color);
        }

        /* ================= TYPOGRAPHY ================= */
        h1, h2, h3 {
            color: #ffffff;
            margin-top: 30px;
            border-bottom: 1px solid var(--border);
            padding-bottom: 0.3em;
        }
        
        h1 { margin-top: 0; border-bottom: none; }
        h1 span { color: var(--accent); }
        h2 { font-size: 1.5em; }
        
        p { color: var(--text-main); }
        b { color: #ffffff; }

        /* ================= HEADER SECTION ================= */
        .header-wrapper {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 30px;
            margin-top: 25px;
            margin-bottom: 30px;
            flex-wrap: wrap; /* Allows stacking on mobile */
        }

        .avatar-container img {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            border: 4px solid var(--accent);
            box-shadow: var(--shadow);
            object-fit: cover;
            /* Animation properties controlled via inline style below */
            animation-name: float;
            animation-iteration-count: infinite;
            animation-timing-function: ease-in-out;
        }

        .header-text {
            text-align: left;
        }

        .role {
            margin-top: 6px;
            font-size: 1.1em;
            color: var(--text-muted);
        }

        /* ================= SECTIONS & IMAGES ================= */
        .content-block {
            text-align: justify;
            margin-bottom: 15px;
        }

        .section-divider {
            border: 0;
            height: 1px;
            background: var(--border);
            margin: 40px 0;
        }

        .image-center {
            display: block;
            margin: 20px auto;
            border-radius: 12px;
            box-shadow: var(--shadow);
            max-width: 100%;
            height: auto;
        }

        .lifecycle-text {
            text-align: center;
            font-family: monospace;
            color: var(--accent);
            background: var(--card-bg);
            padding: 10px;
            border-radius: 6px;
            border: 1px solid var(--border);
        }

        /* ================= SKILLS LISTS ================= */
        ul {
            list-style-type: none;
            padding: 0;
        }

        ul li {
            background: var(--card-bg);
            margin-bottom: 8px;
            padding: 12px 15px;
            border-radius: 6px;
            border-left: 3px solid var(--accent);
        }

        /* ================= BADGES ================= */
        .badge-wrapper {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 10px;
            margin: 20px 0;
        }

        .badge-wrapper img {
            height: auto; /* Maintain aspect ratio */
            max-width: 100%; /* Responsive */
        }

        /* ================= STATS ================= */
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 15px;
            margin-bottom: 30px;
        }

        .stats-grid img {
            width: 100%;
            border-radius: 8px;
        }

        /* ================= ANIMATIONS (KEYFRAMES) ================= */
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }

        @keyframes pulse-border {
            0% { box-shadow: 0 0 0 0 rgba(46, 164, 79, 0.4); }
            70% { box-shadow: 0 0 0 10px rgba(46, 164, 79, 0); }
            100% { box-shadow: 0 0 0 0 rgba(46, 164, 79, 0); }
        }

        /* ================= RESPONSIVE ================= */
        @media (max-width: 600px) {
            .header-wrapper {
                flex-direction: column;
                text-align: center;
            }
            .header-text {
                text-align: center;
            }
        }
    </style>
</head>
<body>

<div class="container">

    <!-- ================= HEADER ================= -->
    <div class="header-wrapper">
        
        <!-- Avatar with Custom Speed Animation (4s float) -->
        <div class="avatar-container">
            <img src="https://media.giphy.com/media/qgQUggAC3Pfv687qPC/giphy.gif"
                 alt="DevOps Profile"
                 style="animation-duration: 4s;" />
        </div>

        <!-- Name + Role -->
        <div class="header-text">
            <h1>Hi 👋, I'm <span style="color:var(--accent);">Vicky Barai</span></h1>
            <p class="role">Aspiring DevOps | MCA Final Year Student</p>
        </div>
    </div>

    <hr class="section-divider"/>

    <!-- ================= ABOUT ================= -->
    <h2>🚀 About Me</h2>

    <div class="content-block">
        <p>
            I am a <b>Vicky Barai</b> and an <b>early-career DevOps </b> actively building
            hands-on experience in Linux, AWS, CI/CD pipelines, containerization, and infrastructure automation.
        </p>
    </div>

    <div class="content-block">
        <p>
            My learning focuses on deploying applications on cloud infrastructure,
            automating build and deployment workflows,
            and managing infrastructure using code.
            I am continuously strengthening my skills through real-world DevOps projects.
        </p>
    </div>

    <div class="content-block">
        <p>
            I believe in <b>automation over repetition</b> and <b>learning by doing</b>.
        </p>
    </div>

    <hr class="section-divider"/>

    <!-- ================= DEVOPS LIFECYCLE ================= -->
    
    <!-- DevOps GIF with Custom Speed Animation (6s float) -->
    <div style="text-align: center;">
        <img src="https://stemettes.org/zine/wp-content/uploads/sites/3/2021/08/DEVOPS.gif"
             alt="DevOps Lifecycle"
             class="image-center"
             style="max-width: 600px; width: 100%; animation: float 6s infinite ease-in-out;" />
    </div>

    <p class="lifecycle-text">
        Plan → Code → Build → Test → Release → Deploy → Operate → Monitor
    </p>

    <hr class="section-divider"/>

    <!-- ================= SKILLS ================= -->
    <h2>🛠️ Skills & Tools</h2>
    <ul>
        <li><b>Operating System:</b> Linux (basic administration, permissions, services)</li>
        <li><b>Cloud:</b> AWS (EC2, S3, IAM, RDS, VPC, CloudWatch)</li>
        <li><b>Version Control:</b> Git, GitHub</li>
        <li><b>CI/CD:</b> Jenkins, GitHub Actions (basic pipelines)</li>
        <li><b>Containers:</b> Docker, Docker Compose, Kubernetes (fundamentals)</li>
        <li><b>Infrastructure as Code:</b> Terraform (basic modules & provisioning)</li>
        <li><b>Scripting:</b> Shell scripting, Python (basics)</li>
    </ul>

    <hr class="section-divider"/>

    <!-- ================= PROJECTS ================= -->
    <h2>🏗️ Projects</h2>

    <h3>🐳 Containerized Web Application</h3>
    <ul>
        <li>Built and containerized a web application using Docker</li>
        <li>Worked with Docker images, containers, volumes, and networks</li>
        <li>Deployed containers on Linux-based cloud instances</li>
    </ul>

    <h3>🔄 CI/CD Pipeline Automation</h3>
    <ul>
        <li>Created basic CI/CD pipelines using Jenkins</li>
        <li>Integrated GitHub repositories with Jenkins jobs</li>
        <li>Automated build and deployment workflows</li>
    </ul>

    <h3>☸️ Kubernetes Deployment (Learning Project)</h3>
    <ul>
        <li>Deployed containerized applications using Kubernetes</li>
        <li>Worked with Pods, Deployments, Services, and basic scaling</li>
        <li>Explored ConfigMaps and Secrets</li>
    </ul>

    <h3>🏗️ Infrastructure Automation with Terraform</h3>
    <ul>
        <li>Provisioned AWS resources using Terraform</li>
        <li>Created EC2 instances and supporting infrastructure</li>
        <li>Worked with Terraform state and reusable configurations</li>
    </ul>

    <hr class="section-divider"/>

    <!-- ================= BADGES & LOGOS ================= -->

    <h2 align="center">🚀 DevOps Skills & Tools</h2>

    <div class="badge-wrapper">
        <!-- OS -->
        <img src="https://img.shields.io/badge/Linux-000000?style=for-the-badge&logo=linux&logoColor=white"/>
        <!-- Cloud -->
        <img src="https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white"/>
        <img src="https://img.shields.io/badge/Amazon%20EC2-FF9900?style=for-the-badge&logo=amazon-ec2&logoColor=white"/>
        <img src="https://img.shields.io/badge/Amazon%20S3-569A31?style=for-the-badge&logo=amazon-s3&logoColor=white"/>
        <img src="https://img.shields.io/badge/IAM-DD344C?style=for-the-badge&logo=amazon-aws&logoColor=white"/>
        <img src="https://img.shields.io/badge/Amazon%20RDS-527FFF?style=for-the-badge&logo=amazon-rds&logoColor=white"/>
        <img src="https://img.shields.io/badge/Amazon%20VPC-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white"/>
        <img src="https://img.shields.io/badge/CloudWatch-FF4F8B?style=for-the-badge&logo=amazon-cloudwatch&logoColor=white"/>
        <!-- DevOps / CI-CD -->
        <img src="https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white"/>
        <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white"/>
        <!-- Containers -->
        <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
        <img src="https://img.shields.io/badge/Docker%20Compose-1488C6?style=for-the-badge&logo=docker&logoColor=white"/>
        <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white"/>
        <!-- IaC -->
        <img src="https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white"/>
        <!-- Version Control -->
        <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white"/>
        <img src="https://img.shields.io/badge/GitHub-121011?style=for-the-badge&logo=github&logoColor=white"/>
        <!-- Scripting -->
        <img src="https://img.shields.io/badge/Shell%20Scripting-4EAA25?style=for-the-badge&logo=gnu-bash&logoColor=white"/>
        <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
    </div>

    <!-- Small Footer Image with Animation -->
    <div style="text-align: center; margin: 30px 0;">
        <img src="https://media.giphy.com/media/LMt9638dO8dftAjtco/giphy.gif"
             alt="DevOps Automation"
             width="200"
             height="200"
             style="border-radius:14px; box-shadow:0 6px 22px rgba(0,0,0,0.3); animation: pulse-border 2s infinite;" />
        <p style="margin-top: 15px; color: var(--accent); font-style: italic;">
            Learning • Building • Automating • Improving
        </p>
    </div>

    <hr class="section-divider"/>

    <!-- ================= STATS SECTION ================= -->
  
    
    <div class="stats-grid">
       # <img src="https://github-readme-stats.vercel.app/api?username=Vickybarai&theme=dark&hide_border=true&include_all_commits=true&count_private=false" alt="GitHub Stats"/>
        <img src="https://nirzak-streak-stats.vercel.app/?user=Vickybarai&theme=dark&hide_border=true" alt="GitHub Streak"/>
        #<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Vickybarai&theme=dark&hide_border=true&include_all_commits=true&count_private=false&layout=compact" alt="Top Languages"/>
        <img src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=radical" alt="DevOps Quote"/>
    </div>

    <!-- ================= BOTTOM IMAGE ================= -->
    <div style="text-align: center; margin-top: 40px;">
        <img src="https://stemettes.org/zine/wp-content/uploads/sites/3/2021/08/6oFTUDQ-1.gif"
             alt="DevOps Automation"
             class="image-center"
             style="max-width: 420px;" />
    </div>

</div>

</body>
</html>
