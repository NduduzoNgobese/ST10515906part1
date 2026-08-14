STUDENT PORTFOLIO PROJECT
ANIRANK 15
Top 15 Shonen Anime Web Application — Project Proposal & Technical Blueprint
1. PROJECT OVERVIEW & SCOPE
Prepared By: Student Software Developer
Course: Software Development Coursework
Version: 1.0 | Date: August 2026
Target Stack: Next.js, Tailwind CSS, Vercel 
AniRank 15 is a focused, high-performance web application designed to catalog, rank, and showcase the Top 15
Shonen Anime Series of all time as complete shows. Developed as a college portfolio project, the application
demonstrates core software engineering principles including responsive UI design, client-side data manipulation,
structured JSON schema handling, and cloud deployment. 
Project Mission: "To build a modern, lightning-fast web application that presents a definitive ranking of
the top 15 Shonen anime series, delivering seamless user interaction, clean dark-mode ergonomics,
and robust code structure suited for professional portfolio showcase." 
1.1 Core Scope Definition
• 
• 
• 
• 
Fixed Dataset: Exactly 15 overall Shonen anime series (evaluated as complete shows, not split into individual
arcs or movies).
Demographic Focus: Strictly Battle/Action Shonen classics (e.g., Fullmetal Alchemist: Brotherhood, Hunter ×
Hunter, One Piece, Naruto, Black Clover).
Architectural Focus: Single-page master ranking grid with interactive sorting, category filtering, responsive
modals, and dark theme UI.
Budget & Infrastructure: 100% free open-source tech stack with zero ongoing hosting costs ($0.00).
2. PROJECT GOALS & LEARNING OBJECTIVES
ACADEMIC & PORTFOLIO GOALS
Showcase 
full-stack 
fundamentals: 
component
architecture, state management, dynamic data rendering,
and clean GitHub repository documentation for potential
employers.
2.1 Key Performance Indicators (KPIs)
METRIC / KPI
Page Load Speed
Lighthouse Performance
Score
BASELINE TARGET
USER EXPERIENCE GOALS
Provide anime fans with instant table sorting (by rank,
rating, episode count), detailed series breakdown modals,
and high-contrast dark mode visuals.
OPTIMIZATION
TARGET
< 1.5 seconds
90 / 100
Mobile Responsiveness
100% functional across
breakpoints
AniRank 15 — Top 15 Shonen Anime Project Proposal
< 0.6 seconds
98+ / 100
Flawless mobile table
layout
EVALUATION METHOD
Google Lighthouse / Vercel
Analytics
Chrome DevTools Audit
Cross-device viewport testing
Page 1 of 5
METRIC / KPI BASELINE TARGET OPTIMIZATION
TARGET EVALUATION METHOD
Deployment &
Infrastructure Cost $0.00 / month $0.00 / month (Free
Tier)
Vercel Starter & GitHub
Pages
3. MASTER CATALOG: TOP 15 SHONEN ANIME SERIES
The table below defines the complete dataset for the application. Each entry represents a complete series
evaluated across animation quality, storytelling, character development, and cultural impact. 
RANK ANIME SERIES TITLE STUDIO EPISODES MAIN POWER SYSTEM /
THEME
MAL
RATING
#1
Fullmetal Alchemist:
Brotherhood Bones 64 Alchemy / Military Fantasy 9.10
#2 Hunter × Hunter (2011) Madhouse 148 Nen / Adventure 9.03
#3 One Piece Toei Animation 1000+ Devil Fruits & Haki / High
Seas 8.72
#4 Gintama Sunrise /
Bandai Namco 367 Samurai / Comedy Action 8.93
#5 Death Note Madhouse 37 Death Notes / Psychological
Thriller 8.62
#6 Jujutsu Kaisen MAPPA 47+ Cursed Energy / Supernatural 8.59
#7
Demon Slayer (Kimetsu no
Yaiba) ufotable 55+ Breathing Styles / Dark
Fantasy 8.74
#8 Attack on Titan Wit Studio /
MAPPA 89 Titan Shifting / Dark Fantasy 8.55
#9 Naruto / Shippuden Studio Pierrot 720 Chakra & Ninjutsu / Shinobi 8.00
#10 Dragon Ball Z Toei Animation 291 Ki & Saiyan Transformations 8.18
#11 Yu Yu Hakusho Studio Pierrot 112 Spirit Energy / Martial Arts 8.46
#12 Black Clover Studio Pierrot 170 Mana & Anti-Magic / Fantasy 8.14
#13 JoJo's Bizarre Adventure David
Production 190 Hamon & Stands /
Supernatural 7.95
#14 My Hero Academia Bones 150+ Quirks / Superhero Action 7.86
#15 Bleach Studio Pierrot 366 Reiryoku & Zanpakuto / Soul
Reapers 7.95
AniRank 15 — Top 15 Shonen Anime Project Proposal Page 2 of 5
4. DATA SCHEMA (`TOP15_SHONEN.JSON`)
To keep backend infrastructure simple and zero-cost, the dataset is defined in a static JSON file loaded directly by
Next.js at build time. 
[
  {
    "rank": 1,
    "title": "Fullmetal Alchemist: Brotherhood",
    "studio": "Bones",
    "episodes": 64,
    "score": 9.10,
    "power_system": "Alchemy",
    "theme": "Military Fantasy / Magic",
    "synopsis": "Two brothers search for the Philosopher's Stone to restore their bodies after 
a failed alchemy ritual.",
    "key_highlight": "Flawless pacing and complete manga adaptation.",
    "poster_url": "/images/fma_brotherhood.jpg"
  },
  {
    "rank": 12,
    "title": "Black Clover",
    "studio": "Studio Pierrot",
    "episodes": 170,
    "score": 8.14,
    "power_system": "Mana & Anti-Magic",
    "theme": "Magic / Fantasy Guilds",
    "synopsis": "Asta, a boy born without magic in a world where magic is everything, aims to 
become the Wizard King.",
    "key_highlight": "Dynamic team battles and relentless protagonist growth.",
    "poster_url": "/images/black_clover.jpg"
  }
]
5. DESIGN & UI SYSTEM
The visual style utilizes a modern Cyber-Anime Dark Theme. High-contrast cards against dark slate backgrounds
reduce eye strain and highlight ratings and rank badges. 
DESIGN ELEMENT
Background (Obsidian)
Container (Card Fill)
Primary Accent
(Crimson)
Secondary Accent
(Amber)
Typography
SPECIFICATION / HEX
CODE
#0F172A (Slate 900)
#1E293B (Slate 800)
#E11D48 (Rose 600)
#F59E0B (Amber 500)
Inter / Montserrat /
Monospaced
AniRank 15 — Top 15 Shonen Anime Project Proposal
APPLICATION
Main application canvas and modal backdrop
Table rows, series cards, and navigation headers
Rank badges, primary CTA buttons, active state indicators
Score highlights, star ratings, and power system tags
Clean sans-serif body text with monospaced numbers for
scores
Page 3 of 5
6. TECHNICAL ARCHITECTURE & TECH STACK
The application is engineered using modern industry-standard web development tools optimized for ease of
learning, high performance, and rapid deployment. 
LAYER
TECHNOLOGY SELECTED RATIONALE FOR STUDENT DEVELOPER
Frontend
Framework
Styling Framework
Next.js 14+ (React)
Tailwind CSS
Automated routing, Server-Side Generation (SSG), fast page
rendering.
Utility-first CSS allowing rapid styling inside JSX without large CSS
files.
Table Data Engine
Version Control
TanStack Table (React
Table)
GitHub
Lightweight engine for client-side sorting (Rank, Rating, Episode
Count).
Industry-standard repository management for code hosting and
commit history.
Deployment
Platform
Vercel (Free Starter Tier)
7. 4-WEEK STUDENT EXECUTION ROADMAP
Structured Weekly Progression: The project is divided into 4 simple 1-week milestones designed to fit
alongside college coursework. 
PHASE
Week 1: Setup &
Data Schema
Week 2: UI & Master
Table
Week 3: Interactive
Features
Week 4: QA & Live
Deployment
MILESTONE DELIVERABLES
Automatic continuous deployment linked directly to the main
GitHub branch.
Initialize Next.js project with Tailwind CSS, create top15_shonen.json
dataset, set up GitHub repository.
Build Navbar, HeroBanner, and main RankTable components mapping
through the 15 series.
Add stateful sorting (by Rank #1–15, MAL Score, Episodes), search filter,
and series detail modal overlay.
Perform mobile viewport testing, optimize Lighthouse performance, deploy to
Vercel, and write README.md portfolio documentation.
8. BUDGET & COST BREAKDOWN
RESOURCE CATEGORY
Code Hosting & Version Control
Web Hosting & Edge CDN
SERVICE PROVIDER
GitHub Public Repository
Vercel Starter Tier
AniRank 15 — Top 15 Shonen Anime Project Proposal
ESTIMATED
HOURS
6–8 hrs
10–12 hrs
8–10 hrs
4–6 hrs
MONTHLY COST
$0.00
$0.00
Page 4 of 5
RESOURCE CATEGORY
SERVICE PROVIDER
MONTHLY COST
Domain Name
Development Tools
Free Vercel Subdomain (.vercel.app)
$0.00
VS Code, Tailwind CSS, Next.js (Open Source)
TOTAL ESTIMATED COST
Student Developer Setup
$0.00
$0.00 / Free
End of Proposal | AniRank 15: Top 15 Shonen Anime Web Application Blueprint | Version 1.0 
AniRank 15 — Top 15 Shonen Anime Project Proposal
Page 5 of 5
