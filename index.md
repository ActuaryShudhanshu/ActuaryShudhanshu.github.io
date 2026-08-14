```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <meta name="description"
        content="Shudhanshu Agarwal - Aspiring Actuarial Analyst">
    <meta name="author" content="Shudhanshu Agarwal">

    <title>Shudhanshu Agarwal | Aspiring Actuarial Analyst</title>

    <!-- Font Awesome CDN -->
    <link rel="stylesheet"
          href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">

    <style>
        :root {
            --navy: #17263c;
            --navy-light: #253956;
            --accent: #287ea8;
            --accent-light: #e9f4f9;
            --text: #293342;
            --muted: #667085;
            --border: #dce3ea;
            --background: #f4f7fa;
            --white: #ffffff;
            --shadow: 0 10px 30px rgba(23, 38, 60, 0.08);
            --radius: 14px;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            line-height: 1.65;
            color: var(--text);
            background: var(--background);
        }

        a {
            color: inherit;
            text-decoration: none;
        }

        .container {
            width: min(1120px, 92%);
            margin: 0 auto;
        }

        /* =========================================
           HEADER
        ========================================= */

        header {
            background: var(--navy);
            color: var(--white);
            padding: 70px 0 55px;
        }

        .header-inner {
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        .profile-section {
            display: flex;
            align-items: center;
            gap: 30px;
        }

        .profile-photo {
            width: 150px;
            height: 150px;
            object-fit: cover;
            border-radius: 50%;
            border: 5px solid rgba(255, 255, 255, 0.95);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.25);
            flex-shrink: 0;
        }

        .profile-info {
            flex: 1;
        }

        .eyebrow {
            color: #8fc7e2;
            font-size: 0.85rem;
            font-weight: 700;
            letter-spacing: 2px;
            text-transform: uppercase;
            margin-bottom: 8px;
        }

        .name {
            font-size: clamp(2.3rem, 6vw, 4.4rem);
            line-height: 1.05;
            font-weight: 800;
            letter-spacing: -1.5px;
        }

        .title {
            font-size: clamp(1.1rem, 2.5vw, 1.45rem);
            font-weight: 400;
            color: #dbe7f0;
            margin-top: 8px;
        }

        .contact-row {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
            margin-top: 10px;
        }

        .contact-item {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            padding: 9px 13px;
            border: 1px solid rgba(255,255,255,0.15);
            border-radius: 8px;
            color: #edf5fa;
            font-size: 0.9rem;
            background: rgba(255,255,255,0.04);
            transition: 0.25s ease;
        }

        .contact-item:hover {
            background: rgba(255,255,255,0.1);
            border-color: #75b9d7;
            transform: translateY(-2px);
        }

        .contact-item i {
            color: #8fc7e2;
            width: 15px;
            text-align: center;
        }

        /* =========================================
           MAIN CONTENT
        ========================================= */

        main {
            padding: 45px 0 70px;
        }

        .section {
            background: var(--white);
            border: 1px solid var(--border);
            border-radius: var(--radius);
            padding: 35px;
            margin-bottom: 25px;
            box-shadow: var(--shadow);
        }

        .section-header {
            display: flex;
            align-items: center;
            gap: 12px;
            margin-bottom: 25px;
        }

        .section-icon {
            width: 38px;
            height: 38px;
            border-radius: 9px;
            display: grid;
            place-items: center;
            background: var(--accent-light);
            color: var(--accent);
            flex-shrink: 0;
        }

        .section-title {
            color: var(--navy);
            font-size: 1.35rem;
            font-weight: 750;
        }

        /* =========================================
           SUMMARY
        ========================================= */

        .summary {
            font-size: 1.04rem;
            color: #465264;
            max-width: 950px;
        }

        /* =========================================
           QUALIFICATIONS TIMELINE
        ========================================= */

        .timeline {
            position: relative;
            margin-left: 6px;
        }

        .timeline::before {
            content: "";
            position: absolute;
            top: 5px;
            bottom: 5px;
            left: 9px;
            width: 2px;
            background: var(--border);
        }

        .timeline-item {
            position: relative;
            display: grid;
            grid-template-columns: 20px 1fr auto;
            gap: 18px;
            margin-bottom: 30px;
            align-items: start;
        }

        .timeline-item:last-child {
            margin-bottom: 0;
        }

        .timeline-dot {
            width: 20px;
            height: 20px;
            background: var(--white);
            border: 5px solid var(--accent);
            border-radius: 50%;
            z-index: 1;
        }

        .timeline-content h3 {
            color: var(--navy);
            font-size: 1.05rem;
            margin-bottom: 3px;
        }

        .timeline-content .institution {
            color: var(--accent);
            font-weight: 700;
            font-size: 0.95rem;
            margin-bottom: 7px;
        }

        .timeline-content p {
            color: var(--muted);
            font-size: 0.92rem;
        }

        .date {
            color: var(--muted);
            font-size: 0.88rem;
            font-weight: 700;
            white-space: nowrap;
            padding-top: 2px;
        }

        .status {
            display: inline-block;
            margin-top: 8px;
            padding: 4px 10px;
            border-radius: 100px;
            background: var(--accent-light);
            color: var(--accent);
            font-size: 0.78rem;
            font-weight: 700;
        }

        /* =========================================
           EDUCATION
        ========================================= */

        .education-grid {
            display: grid;
            grid-template-columns: repeat(2, minmax(0, 1fr));
            gap: 18px;
        }

        .education-card {
            border: 1px solid var(--border);
            border-radius: 12px;
            padding: 20px;
            transition: 0.25s ease;
        }

        .education-card:hover {
            transform: translateY(-3px);
            border-color: #a9cfe1;
            box-shadow: 0 8px 20px rgba(23, 38, 60, 0.06);
        }

        .education-card h3 {
            color: var(--navy);
            font-size: 1rem;
            margin-bottom: 6px;
        }

        .education-card .school {
            color: var(--accent);
            font-weight: 700;
            font-size: 0.92rem;
        }

        .education-card .period {
            margin-top: 7px;
            color: var(--muted);
            font-size: 0.87rem;
        }

        .education-card .result {
            margin-top: 5px;
            font-weight: 700;
            font-size: 0.88rem;
            color: var(--text);
        }

        /* =========================================
           SKILLS
        ========================================= */

        .skill-group {
            margin-bottom: 26px;
        }

        .skill-group:last-child {
            margin-bottom: 0;
        }

        .skill-group-title {
            color: var(--navy);
            font-size: 0.95rem;
            font-weight: 700;
            margin-bottom: 12px;
        }

        .skill-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 9px;
        }

        .skill-tag {
            display: inline-flex;
            align-items: center;
            gap: 7px;
            padding: 8px 13px;
            border: 1px solid #cddbe3;
            border-radius: 100px;
            background: #fbfdfe;
            color: #354052;
            font-size: 0.85rem;
            transition: 0.2s ease;
        }

        .skill-tag:hover {
            border-color: var(--accent);
            color: var(--accent);
            background: var(--accent-light);
        }

        .skill-tag i {
            color: var(--accent);
            font-size: 0.8rem;
        }

        /* =========================================
           LANGUAGES
        ========================================= */

        .language-row {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .language {
            padding: 9px 16px;
            border-radius: 9px;
            background: var(--accent-light);
            color: var(--navy);
            font-weight: 700;
            font-size: 0.9rem;
        }

        /* =========================================
           FOOTER
        ========================================= */

        footer {
            text-align: center;
            padding: 25px 0 35px;
            color: var(--muted);
            font-size: 0.85rem;
        }

        /* =========================================
           PRINT
        ========================================= */

        @media print {
            body {
                background: white;
            }

            header {
                padding: 35px 0;
            }

            main {
                padding: 25px 0;
            }

            .section {
                box-shadow: none;
                break-inside: avoid;
            }

            .contact-item:hover,
            .education-card:hover,
            .skill-tag:hover {
                transform: none;
            }
        }

        /* =========================================
           RESPONSIVE
        ========================================= */

        @media (max-width: 768px) {

            header {
                padding: 45px 0 40px;
            }

            .section {
                padding: 25px 20px;
            }

            .profile-section {
                flex-direction: column;
                align-items: flex-start;
                gap: 20px;
            }

            .profile-photo {
                width: 120px;
                height: 120px;
            }

            .contact-row {
                flex-direction: column;
                align-items: stretch;
            }

            .contact-item {
                width: 100%;
            }

            .timeline-item {
                grid-template-columns: 20px 1fr;
                gap: 12px;
            }

            .date {
                grid-column: 2;
                padding-top: 0;
                margin-top: -6px;
            }

            .education-grid {
                grid-template-columns: 1fr;
            }

            .name {
                letter-spacing: -0.8px;
            }
        }

        @media (max-width: 480px) {

            .container {
                width: min(94%, 1120px);
            }

            main {
                padding: 25px 0 45px;
            }

            .section {
                padding: 22px 17px;
                border-radius: 11px;
            }

            .section-title {
                font-size: 1.2rem;
            }

            .summary {
                font-size: 0.95rem;
            }

            .timeline-content h3 {
                font-size: 0.98rem;
            }

            .contact-item {
                font-size: 0.84rem;
            }

            .skill-tag {
                font-size: 0.8rem;
            }
        }
    </style>
</head>

<body>

    <!-- =========================
         HEADER
    ========================== -->
    <header>
        <div class="container header-inner">

            <div class="profile-section">

                <img
                    src="profile.jpg"
                    alt="Professional portrait of Shudhanshu Agarwal"
                    class="profile-photo"
                >

                <div class="profile-info">

                    <div class="eyebrow">Actuarial Science Professional</div>

                    <h1 class="name">Shudhanshu Agarwal</h1>

                    <p class="title">Aspiring Actuarial Analyst</p>

                </div>

            </div>

            <div class="contact-row">

                <a class="contact-item"
                   href="mailto:agr.shudanshu402@gmail.com">
                    <i class="fa-solid fa-envelope"></i>
                    <span>agr.shudanshu402@gmail.com</span>
                </a>

                <a class="contact-item"
                   href="tel:+916299998089">
                    <i class="fa-solid fa-phone"></i>
                    <span>+91 6299998089</span>
                </a>

                <span class="contact-item">
                    <i class="fa-solid fa-location-dot"></i>
                    <span>Ranchi, Jharkhand</span>
                </span>

                <!-- Add your LinkedIn URL when available -->
                <a class="contact-item"
                   href="https://www.linkedin.com/"
                   target="_blank"
                   rel="noopener noreferrer">
                    <i class="fa-brands fa-linkedin"></i>
                    <span>LinkedIn</span>
                </a>

                <!-- Add your GitHub URL when available -->
                <a class="contact-item"
                   href="https://github.com/"
                   target="_blank"
                   rel="noopener noreferrer">
                    <i class="fa-brands fa-github"></i>
                    <span>GitHub</span>
                </a>

            </div>
        </div>
    </header>


    <!-- =========================
         MAIN
    ========================== -->
    <main>
        <div class="container">

            <!-- SUMMARY -->
            <section class="section">
                <div class="section-header">
                    <div class="section-icon">
                        <i class="fa-solid fa-user-tie"></i>
                    </div>
                    <h2 class="section-title">Professional Summary</h2>
                </div>

                <p class="summary">
                    Aspiring Actuarial Analyst with <strong>CS1 and CM1 cleared from the
                    Institute of Actuaries of India (IAI)</strong> and a strong academic
                    foundation in actuarial science, statistics, mathematics, and financial
                    analysis. Seeking an entry-level actuarial role to apply quantitative
                    and analytical skills in areas such as risk analysis, insurance,
                    reserving, pricing, and data analysis while gaining hands-on industry
                    experience and progressing toward actuarial qualification.
                </p>
            </section>


            <!-- ACTUARIAL QUALIFICATIONS -->
            <section class="section">
                <div class="section-header">
                    <div class="section-icon">
                        <i class="fa-solid fa-chart-line"></i>
                    </div>
                    <h2 class="section-title">Actuarial Qualification Journey</h2>
                </div>

                <div class="timeline">

                    <div class="timeline-item">
                        <div class="timeline-dot"></div>

                        <div class="timeline-content">
                            <h3>CM1 — Actuarial Mathematics</h3>
                            <div class="institution">
                                Institute of Actuaries of India (IAI)
                            </div>
                            <p>
                                Cleared the Actuarial Mathematics examination,
                                demonstrating a foundation in financial mathematics
                                and actuarial modelling concepts.
                            </p>

                            <span class="status">
                                <i class="fa-solid fa-circle-check"></i>
                                Passed
                            </span>
                        </div>

                        <div class="date">Nov 2025</div>
                    </div>


                    <div class="timeline-item">
                        <div class="timeline-dot"></div>

                        <div class="timeline-content">
                            <h3>CS1 — Actuarial Statistics</h3>
                            <div class="institution">
                                Institute of Actuaries of India (IAI)
                            </div>
                            <p>
                                Cleared the Actuarial Statistics examination,
                                building a foundation in probability, statistics
                                and quantitative analysis.
                            </p>

                            <span class="status">
                                <i class="fa-solid fa-circle-check"></i>
                                Passed
                            </span>
                        </div>

                        <div class="date">May 2025</div>
                    </div>


                    <div class="timeline-item">
                        <div class="timeline-dot"></div>

                        <div class="timeline-content">
                            <h3>ACET — Actuarial Common Entrance Exam</h3>
                            <div class="institution">
                                Institute of Actuaries of India (IAI)
                            </div>
                            <p>
                                Successfully cleared the entrance examination
                                for the actuarial profession.
                            </p>

                            <span class="status">
                                <i class="fa-solid fa-circle-check"></i>
                                Passed
                            </span>
                        </div>

                        <div class="date">Dec 2024</div>
                    </div>


                    <div class="timeline-item">
                        <div class="timeline-dot"></div>

                        <div class="timeline-content">
                            <h3>Current Actuarial Studies</h3>
                            <div class="institution">
                                Institute of Actuaries of India (IAI)
                            </div>
                            <p>
                                Currently preparing for <strong>CM2</strong> and
                                <strong>CB1</strong>.
                            </p>
                        </div>

                        <div class="date">Current</div>
                    </div>

                </div>
            </section>


            <!-- EDUCATION -->
            <section class="section">
                <div class="section-header">
                    <div class="section-icon">
                        <i class="fa-solid fa-graduation-cap"></i>
                    </div>
                    <h2 class="section-title">Education</h2>
                </div>

                <div class="education-grid">

                    <article class="education-card">

                        <h3>M.Sc. Actuarial Science</h3>

                        <div class="school">
                            Amity University Noida
                        </div>

                        <div class="period">
                            2026 – 2028
                        </div>

                    </article>


                    <article class="education-card">

                        <h3>B.Com (Honors), Accountancy</h3>

                        <div class="school">
                            Ranchi University
                        </div>

                        <div class="period">
                            2021 – 2024
                        </div>

                        <div class="result">
                            CGPA: 8.3
                        </div>

                    </article>


                    <article class="education-card">

                        <h3>Higher Secondary (12th)</h3>

                        <div class="school">
                            DAV Public School
                        </div>

                        <div class="period">
                            2019 – 2021
                        </div>

                        <div class="result">
                            84.2%
                        </div>

                    </article>

                </div>
            </section>


            <!-- TECHNICAL SKILLS -->
            <section class="section">
                <div class="section-header">
                    <div class="section-icon">
                        <i class="fa-solid fa-laptop-code"></i>
                    </div>
                    <h2 class="section-title">Technical Skills</h2>
                </div>


                <div class="skill-group">

                    <div class="skill-group-title">
                        Excel
                    </div>

                    <div class="skill-tags">

                        <span class="skill-tag">
                            <i class="fa-solid fa-table"></i>
                            Data Cleaning
                        </span>

                        <span class="skill-tag">
                            <i class="fa-solid fa-table"></i>
                            Pivot Tables
                        </span>

                        <span class="skill-tag">
                            <i class="fa-solid fa-magnifying-glass-chart"></i>
                            VLOOKUP / XLOOKUP
                        </span>

                        <span class="skill-tag">
                            <i class="fa-solid fa-gears"></i>
                            Macros
                        </span>

                        <span class="skill-tag">
                            <i class="fa-solid fa-calculator"></i>
                            Financial Calculations
                        </span>

                    </div>
                </div>


                <div class="skill-group">

                    <div class="skill-group-title">
                        R Programming
                    </div>

                    <div class="skill-tags">

                        <span class="skill-tag">
                            <i class="fa-solid fa-chart-column"></i>
                            Data Manipulation
                        </span>

                        <span class="skill-tag">
                            <i class="fa-solid fa-chart-line"></i>
                            Statistical Analysis
                        </span>

                        <span class="skill-tag">
                            <i class="fa-solid fa-chart-area"></i>
                            Regression Fundamentals
                        </span>

                    </div>
                </div>


                <div class="skill-group">

                    <div class="skill-group-title">
                        Python
                    </div>

                    <div class="skill-tags">

                        <span class="skill-tag">
                            <i class="fa-brands fa-python"></i>
                            Scripting Fundamentals
                        </span>

                        <span class="skill-tag">
                            <i class="fa-solid fa-code"></i>
                            Data Structures
                        </span>

                        <span class="skill-tag">
                            <i class="fa-solid fa-seedling"></i>
                            Beginner Level
                        </span>

                    </div>
                </div>


                <div class="skill-group">

                    <div class="skill-group-title">
                        Actuarial Concepts
                    </div>

                    <div class="skill-tags">

                        <span class="skill-tag">
                            <i class="fa-solid fa-chart-line"></i>
                            CM1 Concepts
                        </span>

                        <span class="skill-tag">
                            <i class="fa-solid fa-square-root-variable"></i>
                            CS1 Concepts
                        </span>

                        <span class="skill-tag">
                            <i class="fa-solid fa-coins"></i>
                            Financial Mathematics
                        </span>

                        <span class="skill-tag">
                            <i class="fa-solid fa-dice"></i>
                            Probability
                        </span>

                        <span class="skill-tag">
                            <i class="fa-solid fa-scale-balanced"></i>
                            Basic Valuation Principles
                        </span>

                    </div>
                </div>

            </section>


            <!-- SOFT SKILLS -->
            <section class="section">

                <div class="section-header">
                    <div class="section-icon">
                        <i class="fa-solid fa-people-group"></i>
                    </div>
                    <h2 class="section-title">Professional Skills</h2>
                </div>

                <div class="skill-tags">

                    <span class="skill-tag">
                        <i class="fa-solid fa-brain"></i>
                        Analytical Thinking
                    </span>

                    <span class="skill-tag">
                        <i class="fa-solid fa-puzzle-piece"></i>
                        Problem Solving
                    </span>

                    <span class="skill-tag">
                        <i class="fa-solid fa-magnifying-glass"></i>
                        Attention to Detail
                    </span>

                    <span class="skill-tag">
                        <i class="fa-solid fa-arrows-rotate"></i>
                        Adaptability
                    </span>

                    <span class="skill-tag">
                        <i class="fa-solid fa-book-open"></i>
                        Willingness to Learn
                    </span>

                    <span class="skill-tag">
                        <i class="fa-solid fa-users"></i>
                        Team Collaboration
                    </span>

                </div>

            </section>


            <!-- LANGUAGES -->
            <section class="section">

                <div class="section-header">
                    <div class="section-icon">
                        <i class="fa-solid fa-language"></i>
                    </div>
                    <h2 class="section-title">Languages</h2>
                </div>

                <div class="language-row">

                    <span class="language">
                        English
                    </span>

                    <span class="language">
                        Hindi
                    </span>

                </div>

            </section>

        </div>
    </main>


    <!-- FOOTER -->
    <footer>
        <div class="container">
            © <span id="year"></span> Shudhanshu Agarwal · Aspiring Actuarial Analyst
        </div>
    </footer>


    <script>
        // Automatically update footer year
        document.getElementById("year").textContent = new Date().getFullYear();
    </script>

</body>
</html>
```