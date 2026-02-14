<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NagendranSanjeevan · attractive dev profile</title>
    <!-- Font Awesome 6 (free) for clean icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <!-- Google Fonts: Inter + space for code vibe -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,400;14..32,500;14..32,600;14..32,700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: linear-gradient(145deg, #f0f4fa 0%, #e6ecf5 100%);
            font-family: 'Inter', system-ui, -apple-system, sans-serif;
            display: flex;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
            padding: 1.5rem;
            margin: 0;
            color: #1a2639;
        }

        .card {
            max-width: 1000px;
            width: 100%;
            background: rgba(255, 255, 255, 0.75);
            backdrop-filter: blur(14px);
            -webkit-backdrop-filter: blur(14px);
            border-radius: 3rem 2rem 3rem 2rem;
            box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.2), inset 0 1px 2px rgba(255,255,255,0.8);
            padding: 2.2rem 2.5rem;
            border: 1px solid rgba(255,255,255,0.6);
            transition: all 0.2s ease;
        }

        /* header with wave */
        .profile-head {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            gap: 1.8rem;
            margin-bottom: 2rem;
        }

        .avatar-badge {
            background: linear-gradient(125deg, #0b2b40, #1d4e6f);
            width: 85px;
            height: 85px;
            border-radius: 40% 60% 30% 70% / 50% 40% 60% 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 12px 18px -8px rgba(0,40,70,0.4);
            border: 3px solid white;
        }

        .avatar-badge span {
            font-size: 3rem;
            filter: drop-shadow(2px 4px 4px rgba(0,0,0,0.2));
        }

        .name-title h1 {
            font-size: 2.8rem;
            font-weight: 700;
            letter-spacing: -0.02em;
            line-height: 1.1;
            background: linear-gradient(130deg, #1f3a4b, #2d5670);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            display: flex;
            align-items: center;
            gap: 0.3rem;
        }

        .name-title h1 i {
            font-size: 2.6rem;
            background: none;
            -webkit-text-fill-color: #3f6b8f;
            color: #3f6b8f;
        }

        .tagline {
            margin-top: 0.3rem;
            display: flex;
            gap: 1.2rem;
            flex-wrap: wrap;
            color: #2d4356;
            font-weight: 500;
        }

        .tagline span {
            background: rgba(44, 82, 110, 0.08);
            padding: 0.3rem 1rem 0.3rem 0.8rem;
            border-radius: 40px;
            display: inline-flex;
            align-items: center;
            gap: 8px;
            font-size: 0.95rem;
            border: 1px solid rgba(255,255,255,0.7);
            backdrop-filter: blur(4px);
        }

        .tagline i {
            color: #1f5978;
            font-size: 1rem;
        }

        .reach-out {
            margin-left: auto;
            background: #ffffffcc;
            border-radius: 100px;
            padding: 0.7rem 1.7rem 0.7rem 1.4rem;
            box-shadow: 0 8px 14px rgba(0,32,54,0.1);
            border: 1px solid rgba(255,255,255,0.9);
            display: flex;
            align-items: center;
            gap: 10px;
            font-weight: 600;
            color: #113946;
            transition: 0.15s;
        }

        .reach-out i {
            font-size: 1.4rem;
            color: #236b9c;
        }

        .reach-out a {
            text-decoration: none;
            color: #153e54;
            border-bottom: 2px dotted #8db3d0;
        }

        .reach-out a:hover {
            border-bottom: 2px solid #236b9c;
        }

        /* connect section */
        .connect-strip {
            display: flex;
            align-items: center;
            gap: 1rem;
            margin: 1.8rem 0 2rem 0;
            background: #eef3f8dd;
            border-radius: 80px;
            padding: 0.6rem 1.8rem 0.6rem 2rem;
            border: 1px solid #ffffff;
            width: fit-content;
            backdrop-filter: blur(4px);
        }

        .connect-strip h3 {
            font-size: 1.2rem;
            font-weight: 600;
            color: #0f3549;
            letter-spacing: -0.2px;
        }

        .social-links {
            display: flex;
            gap: 1.1rem;
        }

        .social-links a {
            background: white;
            width: 38px;
            height: 38px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #215d81;
            font-size: 1.3rem;
            box-shadow: 0 6px 12px rgba(0, 30, 50, 0.1);
            transition: all 0.2s;
            border: 1px solid rgba(255,255,255,0.7);
        }

        .social-links a:hover {
            background: #215d81;
            color: white;
            transform: translateY(-4px) scale(1.05);
        }

        /* languages & tools */
        .tools-section {
            margin: 2.5rem 0 2rem 0;
        }

        .section-label {
            display: flex;
            align-items: center;
            gap: 0.6rem;
            font-weight: 700;
            font-size: 1.4rem;
            color: #183f56;
            margin-bottom: 1.2rem;
            border-left: 8px solid #367f9e;
            padding-left: 1.2rem;
        }

        .tool-icons {
            display: flex;
            gap: 1.2rem;
            flex-wrap: wrap;
        }

        .tool-badge {
            background: #ffffffd6;
            backdrop-filter: blur(4px);
            border-radius: 80px;
            padding: 0.7rem 2rem 0.7rem 1.8rem;
            display: flex;
            align-items: center;
            gap: 12px;
            font-weight: 600;
            font-size: 1.1rem;
            color: #1e4b68;
            box-shadow: 0 8px 18px -10px #0f3550;
            border: 1px solid white;
            transition: 0.12s;
        }

        .tool-badge i {
            font-size: 1.6rem;
            color: #2e6182;
        }

        .tool-badge:hover {
            background: white;
            box-shadow: 0 12px 20px -12px #0a283a;
            transform: scale(1.02);
        }

        /* repositories grid */
        .repo-header {
            display: flex;
            justify-content: space-between;
            align-items: baseline;
            margin: 2.5rem 0 1rem 0;
        }

        .repo-header h2 {
            font-weight: 700;
            font-size: 1.8rem;
            background: linear-gradient(145deg, #1c445b, #30627e);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .customize-note {
            background: #dbe9f3;
            padding: 0.35rem 1.3rem;
            border-radius: 40px;
            font-weight: 600;
            font-size: 0.9rem;
            color: #194358;
            display: flex;
            align-items: center;
            gap: 8px;
            border: 1px solid #ffffff;
        }

        .repo-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1.2rem;
            margin: 1.5rem 0 0.8rem 0;
        }

        .repo-card {
            background: #ffffffbf;
            backdrop-filter: blur(8px);
            border-radius: 2rem 1.2rem 2rem 1.2rem;
            padding: 1.4rem 1.2rem 1.2rem 1.5rem;
            border: 1px solid rgba(255,255,255,0.9);
            transition: 0.15s;
            box-shadow: 0 12px 22px -18px #102c3b;
        }

        .repo-card:hover {
            background: white;
            transform: translateY(-5px);
            border-color: #b1d0e3;
            box-shadow: 0 22px 28px -18px #06212e;
        }

        .repo-name {
            display: flex;
            align-items: center;
            gap: 10px;
            font-weight: 700;
            font-size: 1.3rem;
            color: #154152;
        }

        .repo-name i {
            font-size: 1.3rem;
            color: #387aa3;
        }

        .repo-desc {
            margin-top: 12px;
            font-size: 0.9rem;
            color: #2e4b60;
            font-weight: 500;
            border-left: 2px solid #87b9d3;
            padding-left: 12px;
        }

        .repo-meta {
            margin-top: 16px;
            display: flex;
            gap: 1rem;
            font-size: 0.8rem;
            font-weight: 600;
            color: #2e6582;
        }

        .pin-footer {
            margin-top: 2rem;
            text-align: right;
            display: flex;
            align-items: center;
            justify-content: space-between;
            border-top: 2px dashed #b3ccdf;
            padding-top: 1.5rem;
            flex-wrap: wrap;
        }

        .pin-footer span {
            font-weight: 600;
            color: #1f4f6e;
            background: #dfecf5;
            padding: 0.4rem 1.6rem;
            border-radius: 60px;
            font-size: 0.95rem;
            display: inline-flex;
            align-items: center;
            gap: 10px;
            border: 1px solid white;
        }

        .pin-footer small {
            color: #386883;
            font-weight: 500;
        }

        hr {
            border: 1px solid rgba(151, 187, 212, 0.3);
            margin: 1rem 0;
        }

        /* responsiveness */
        @media (max-width: 700px) {
            .card { padding: 1.8rem; }
            .name-title h1 { font-size: 2.2rem; }
            .profile-head { gap: 1rem; }
            .reach-out { margin-left: 0; width: 100%; }
        }
    </style>
</head>
<body>
    <div class="card">

        <!-- header with name + 👋 -->
        <div class="profile-head">
            <div class="avatar-badge">
                <span>👋</span>
            </div>
            <div class="name-title">
                <h1>
                    I'm NagendranSanjeevan 
                    <i class="fa-regular fa-hand-peace"></i>
                </h1>
                <div class="tagline">
                    <span><i class="fa-solid fa-brain"></i> learning ML & Figma</span>
                    <span><i class="fa-regular fa-envelope"></i> nagendransanjeewa3060@gmail.com</span>
                </div>
            </div>
            <div class="reach-out">
                <i class="fa-regular fa-paper-plane"></i>
                <span><a href="mailto:nagendransanjeewa3060@gmail.com">reach me</a> 🛜</span>
            </div>
        </div>

        <!-- Connect section with icons (even if no explicit links, we illustrate) -->
        <div class="connect-strip">
            <h3><i class="fa-regular fa-compass"></i> Connect with me:</h3>
            <div class="social-links">
                <a href="#" aria-label="github"><i class="fa-brands fa-github"></i></a>
                <a href="#" aria-label="linkedin"><i class="fa-brands fa-linkedin-in"></i></a>
                <a href="#" aria-label="figma"><i class="fa-brands fa-figma"></i></a>
                <a href="#" aria-label="x"><i class="fa-brands fa-x-twitter"></i></a>
            </div>
        </div>

        <!-- Languages and tools (AWS, .NET, MySQL) with more attractive style -->
        <div class="tools-section">
            <div class="section-label">
                <i class="fa-solid fa-code"></i>  languages & tools
            </div>
            <div class="tool-icons">
                <div class="tool-badge"><i class="fa-brands fa-aws"></i> AWS</div>
                <div class="tool-badge"><i class="fa-brands fa-microsoft"></i> Microsoft .NET</div>
                <div class="tool-badge"><i class="fa-solid fa-database"></i> MySQL</div>
                <!-- plus an extra fun one: -->
                <div class="tool-badge"><i class="fa-regular fa-file-code"></i> Figma</div>
            </div>
        </div>

        <!-- Popular repositories + pin customization -->
        <div class="repo-header">
            <h2><i class="fa-regular fa-star" style="margin-right: 8px;"></i> Popular repositories</h2>
            <div class="customize-note">
                <i class="fa-regular fa-pen-to-square"></i> Customize your pins
            </div>
        </div>

        <!-- repo grid using given names: gitupemc1, merge2, GitHub, Lastcheck (and we add small touches) -->
        <div class="repo-grid">
            <!-- gitupemc1 -->
            <div class="repo-card">
                <div class="repo-name"><i class="fa-regular fa-folder-open"></i> gitupemc1</div>
                <div class="repo-desc">⚡ emC + git utilities · fresh workflow</div>
                <div class="repo-meta"><i class="fa-regular fa-circle-dot"></i> 14 stars <span style="margin-left: auto;"><i class="fa-regular fa-code-merge"></i> 3</span></div>
            </div>
            <!-- merge2 -->
            <div class="repo-card">
                <div class="repo-name"><i class="fa-regular fa-code-merge"></i> merge2</div>
                <div class="repo-desc">🔀 smart merging & conflict assistant</div>
                <div class="repo-meta"><i class="fa-regular fa-star"></i> 27 <span style="margin-left: auto;"><i class="fa-regular fa-code-branch"></i> 8</span></div>
            </div>
            <!-- GitHub (repo) -->
            <div class="repo-card">
                <div class="repo-name"><i class="fa-brands fa-github"></i> GitHub</div>
                <div class="repo-desc">🐙 octopus sandbox · pinned</div>
                <div class="repo-meta"><i class="fa-regular fa-star"></i> 132 <span style="margin-left: auto;"><i class="fa-regular fa-clock"></i> updated 2d</span></div>
            </div>
            <!-- Lastcheck -->
            <div class="repo-card">
                <div class="repo-name"><i class="fa-regular fa-check-circle"></i> Lastcheck</div>
                <div class="repo-desc">✅ final validation & monitoring tool</div>
                <div class="repo-meta"><i class="fa-regular fa-eye"></i> 9 <span style="margin-left: auto;"><i class="fa-regular fa-calendar"></i> Mar 2025</span></div>
            </div>
        </div>

        <!-- extra pins footer to reinforce "Customize your pins" -->
        <div class="pin-footer">
            <span><i class="fa-regular fa-thumbtack"></i> 4 pinned repositories</span>
            <small>⭐ you can rearrange · <i class="fa-regular fa-pen-to-square"></i> edit pins</small>
        </div>

        <!-- subtle hr, then more personal learning line (already in header, but just to mirror original "I’m currently learning..." ) -->
        <hr>
        <div style="display: flex; gap: 2rem; flex-wrap: wrap; justify-content: space-between; align-items: center;">
            <div style="display: flex; gap: 0.8rem;">
                <i class="fa-solid fa-arrow-trend-up" style="color:#306e93;"></i>
                <span style="font-weight: 500;"># currently diving deeper: <span style="background: #cddde9; padding:0.3rem 0.9rem; border-radius:40px;">ML • Figma • .NET 9</span></span>
            </div>
            <div style="color:#2f688b;">
                <i class="fa-regular fa-message"></i> nagendransanjeewa3060@gmail.com
            </div>
        </div>

        <!-- tiny design line: all original info present in much more attractive layout  ✅ -->
    </div>
</body>
</html>
