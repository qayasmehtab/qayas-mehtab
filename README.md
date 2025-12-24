<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Qayas Mehtab | Cloud Data Engineer Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&family=Fira+Code:wght@400;500&display=swap');
        body { font-family: 'Inter', sans-serif; background-color: #020617; color: #f8fafc; scroll-behavior: smooth; }
        .glass { background: rgba(15, 23, 42, 0.8); backdrop-filter: blur(12px); border: 1px solid rgba(255,255,255,0.1); }
        .gradient-text { background: linear-gradient(135deg, #38bdf8 0%, #818cf8 50%, #c084fc 100%); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }
        .card-hover { transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1); }
        .card-hover:hover { transform: translateY(-10px); border-color: #38bdf8; box-shadow: 0 20px 40px -20px rgba(56, 189, 248, 0.4); }
        
        /* Cyber-Tech Banner Background */
        .tech-banner {
            background: radial-gradient(circle at 50% 50%, #1e293b 0%, #020617 100%);
            position: relative;
            overflow: hidden;
        }
        .grid-overlay {
            position: absolute;
            inset: 0;
            background-image: linear-gradient(rgba(56, 189, 248, 0.05) 1px, transparent 1px), linear-gradient(90deg, rgba(56, 189, 248, 0.05) 1px, transparent 1px);
            background-size: 50px 50px;
            perspective: 1000px;
            transform: rotateX(60deg) translateY(-100px);
            z-index: 0;
        }
        .floating { animation: float 6s ease-in-out infinite; }
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
        }
        .pulse-border { animation: pulse 2s infinite; }
        @keyframes pulse {
            0% { box-shadow: 0 0 0 0 rgba(56, 189, 248, 0.4); }
            70% { box-shadow: 0 0 0 15px rgba(56, 189, 248, 0); }
            100% { box-shadow: 0 0 0 0 rgba(56, 189, 248, 0); }
        }
    </style>
</head>
<body>

    <!-- Navbar -->
    <nav class="fixed w-full z-50 glass border-b border-white/5">
        <div class="max-w-7xl mx-auto px-6 py-4 flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <div class="w-8 h-8 bg-sky-500 rounded-lg flex items-center justify-center font-black text-white italic">Q</div>
                <span class="text-xl font-bold tracking-tighter">QAYAS MEHTAB</span>
            </div>
            <div class="hidden md:flex space-x-8 text-[10px] font-bold uppercase tracking-widest">
                <a href="#skills" class="hover:text-sky-400 transition">Skills</a>
                <a href="#projects" class="hover:text-sky-400 transition">Repositories</a>
                <a href="#contact" class="px-4 py-2 bg-sky-500 rounded-md text-white hover:bg-sky-400 transition">Contact Me</a>
            </div>
        </div>
    </nav>

    <!-- Professional Tech Banner (Hero) -->
    <section class="tech-banner min-h-screen flex items-center justify-center pt-20 px-6">
        <div class="grid-overlay"></div>
        
        <div class="max-w-7xl w-full grid lg:grid-cols-2 gap-16 items-center z-10">
            <!-- Left Side: Professional Hook -->
            <div class="text-center lg:text-left">
                <div class="inline-flex items-center space-x-3 bg-white/5 border border-white/10 px-4 py-2 rounded-full mb-8">
                    <span class="w-2 h-2 rounded-full bg-sky-500 animate-pulse"></span>
                    <span class="text-[10px] font-bold uppercase tracking-[0.2em] text-slate-300">Operational Excellence &rarr; Data Engineering</span>
                </div>
                
                <h1 class="text-6xl md:text-8xl font-black mb-6 tracking-tighter leading-none">
                    Building <br> <span class="gradient-text italic">Data Highways</span>
                </h1>
                
                <p class="text-slate-400 text-lg md:text-xl mb-10 max-w-xl font-medium leading-relaxed">
                    Cloud Data Engineer focused on <span class="text-white underline decoration-sky-500 decoration-2 underline-offset-4">ETL Pipelines</span>, Web Scraping, and scalable Database Architectures. 
                </p>

                <div class="flex flex-wrap justify-center lg:justify-start gap-4">
                    <a href="#projects" class="px-8 py-4 bg-white text-black font-black rounded-xl hover:bg-sky-400 hover:text-white transition-all transform hover:scale-105 active:scale-95 flex items-center">
                        <i class="fa-brands fa-github mr-2"></i> Explore Code
                    </a>
                    <a href="https://linkedin.com/in/qayas" target="_blank" class="px-8 py-4 glass text-white font-bold rounded-xl border border-white/10 hover:border-sky-500 transition-all flex items-center">
                        <i class="fa-brands fa-linkedin-in mr-2 text-sky-400"></i> LinkedIn
                    </a>
                </div>
            </div>

            <!-- Right Side: The "Visual Banner" Card -->
            <div class="relative group">
                <!-- Decorative Glows -->
                <div class="absolute -inset-1 bg-gradient-to-r from-sky-500 to-indigo-500 rounded-[2rem] blur opacity-25 group-hover:opacity-50 transition duration-1000"></div>
                
                <div class="glass p-1 rounded-[2rem] border-white/10 shadow-2xl overflow-hidden">
                    <div class="bg-slate-950/80 p-8 md:p-12 rounded-[1.8rem]">
                        <!-- Visual Header -->
                        <div class="flex justify-between items-start mb-10">
                            <div>
                                <h3 class="text-2xl font-black text-white tracking-tighter mb-1">DATA_PIPELINE.v1</h3>
                                <div class="flex space-x-1">
                                    <span class="h-1 w-8 bg-sky-500 rounded-full"></span>
                                    <span class="h-1 w-4 bg-indigo-500 rounded-full"></span>
                                </div>
                            </div>
                            <i class="fa-solid fa-cloud-arrow-down text-3xl text-sky-500/50"></i>
                        </div>

                        <!-- Skill Tags Overlay -->
                        <div class="space-y-6">
                            <div class="flex flex-wrap gap-3">
                                <span class="px-3 py-1 bg-sky-500/10 border border-sky-500/20 rounded-md text-[10px] font-bold text-sky-400 tracking-widest uppercase">Python</span>
                                <span class="px-3 py-1 bg-indigo-500/10 border border-indigo-500/20 rounded-md text-[10px] font-bold text-indigo-400 tracking-widest uppercase">SQL Server</span>
                                <span class="px-3 py-1 bg-emerald-500/10 border border-emerald-500/20 rounded-md text-[10px] font-bold text-emerald-400 tracking-widest uppercase">Snowflake</span>
                                <span class="px-3 py-1 bg-purple-500/10 border border-purple-500/20 rounded-md text-[10px] font-bold text-purple-400 tracking-widest uppercase">AWS</span>
                            </div>

                            <!-- Live Code Snippet -->
                            <div class="font-mono text-[12px] p-6 bg-black/40 rounded-2xl border border-white/5 leading-loose">
                                <div class="flex space-x-2 mb-2">
                                    <div class="w-2 h-2 rounded-full bg-red-400"></div>
                                    <div class="w-2 h-2 rounded-full bg-yellow-400"></div>
                                    <div class="w-2 h-2 rounded-full bg-green-400"></div>
                                </div>
                                <p><span class="text-purple-400">def</span> <span class="text-sky-400">etl_process</span>():</p>
                                <p class="pl-4"><span class="text-slate-500"># Scraping Market Data</span></p>
                                <p class="pl-4 text-emerald-400">raw_data = scraper.get_pakwheels()</p>
                                <p class="pl-4 text-slate-300">clean_df = transform(raw_data)</p>
                                <p class="pl-4"><span class="text-sky-400 text-opacity-70 italic">db.load(clean_df, warehouse='Snowflake')</span></p>
                            </div>
                            
                            <!-- Stats -->
                            <div class="flex justify-between items-center pt-4">
                                <div class="text-center">
                                    <div class="text-2xl font-black text-white">7+</div>
                                    <div class="text-[9px] font-bold text-slate-500 uppercase tracking-tighter">Years Ops Exp</div>
                                </div>
                                <div class="h-8 w-[1px] bg-white/10"></div>
                                <div class="text-center">
                                    <div class="text-2xl font-black text-sky-400">100%</div>
                                    <div class="text-[9px] font-bold text-slate-500 uppercase tracking-tighter">Automation Goal</div>
                                </div>
                                <div class="h-8 w-[1px] bg-white/10"></div>
                                <div class="text-center">
                                    <div class="text-2xl font-black text-white">SQL</div>
                                    <div class="text-[9px] font-bold text-slate-500 uppercase tracking-tighter">Mastery</div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Technical Skills Grid -->
    <section id="skills" class="py-24 px-6 max-w-7xl mx-auto">
        <div class="text-center mb-16">
            <h2 class="text-sm font-bold text-sky-500 tracking-[0.4em] uppercase mb-4">Core Competencies</h2>
            <p class="text-3xl md:text-5xl font-black tracking-tight">Tools of the <span class="gradient-text">Trade</span></p>
        </div>
        
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
            <!-- Skill Block -->
            <div class="glass p-10 rounded-[2.5rem] card-hover text-center">
                <div class="w-20 h-20 bg-sky-500/10 rounded-3xl flex items-center justify-center mx-auto mb-6">
                    <i class="fa-brands fa-python text-4xl text-sky-500"></i>
                </div>
                <h4 class="text-xl font-bold mb-2">Python</h4>
                <p class="text-slate-500 text-sm">ETL Frameworks, Pandas, Automation Scripts</p>
            </div>
            
            <div class="glass p-10 rounded-[2.5rem] card-hover text-center">
                <div class="w-20 h-20 bg-indigo-500/10 rounded-3xl flex items-center justify-center mx-auto mb-6">
                    <i class="fa-solid fa-database text-4xl text-indigo-500"></i>
                </div>
                <h4 class="text-xl font-bold mb-2">SQL Engineering</h4>
                <p class="text-slate-500 text-sm">Complex Queries, SQL Server, Snowflake Warehousing</p>
            </div>

            <div class="glass p-10 rounded-[2.5rem] card-hover text-center">
                <div class="w-20 h-20 bg-emerald-500/10 rounded-3xl flex items-center justify-center mx-auto mb-6">
                    <i class="fa-solid fa-robot text-4xl text-emerald-500"></i>
                </div>
                <h4 class="text-xl font-bold mb-2">Web Scraping</h4>
                <p class="text-slate-500 text-sm">Selenium, BeautifulSoup, Data Extraction</p>
            </div>

            <div class="glass p-10 rounded-[2.5rem] card-hover text-center">
                <div class="w-20 h-20 bg-purple-500/10 rounded-3xl flex items-center justify-center mx-auto mb-6">
                    <i class="fa-solid fa-cloud-bolt text-4xl text-purple-500"></i>
                </div>
                <h4 class="text-xl font-bold mb-2">Cloud Infrastructure</h4>
                <p class="text-slate-500 text-sm">AWS Integration, Pipeline Deployment</p>
            </div>
        </div>
    </section>

    <!-- GitHub Showcase Section -->
    <section id="projects" class="py-24 px-6 bg-slate-950/50">
        <div class="max-w-7xl mx-auto">
            <div class="flex flex-col md:flex-row justify-between items-end mb-16 gap-6">
                <div>
                    <h2 class="text-sm font-bold text-sky-500 tracking-[0.4em] uppercase mb-4">Open Source Repositories</h2>
                    <p class="text-3xl md:text-5xl font-black tracking-tight">Recent <span class="gradient-text">Projects</span></p>
                </div>
                <a href="https://github.com/qayasmehtab" target="_blank" class="px-6 py-3 border border-white/10 rounded-xl font-bold text-sm hover:bg-white hover:text-black transition-all">View All on GitHub <i class="fa-brands fa-github ml-2"></i></a>
            </div>

            <div class="grid lg:grid-cols-2 gap-8">
                <!-- Project Card 1 -->
                <div class="glass p-8 md:p-12 rounded-[3rem] card-hover group border-l-8 border-sky-500">
                    <div class="flex justify-between items-start mb-8">
                        <div class="w-12 h-12 bg-sky-500 rounded-2xl flex items-center justify-center text-white">
                            <i class="fa-solid fa-gears text-2xl"></i>
                        </div>
                        <span class="text-[10px] font-black text-sky-400 bg-sky-500/10 px-3 py-1 rounded-full uppercase">Live Repo</span>
                    </div>
                    <h4 class="text-2xl font-black mb-4 group-hover:text-sky-400 transition">Python ETL Framework</h4>
                    <p class="text-slate-400 mb-8 leading-relaxed">
                        A complete framework for building modular ETL pipelines. Includes custom logging, error handling, and multi-format data loaders.
                    </p>
                    <div class="flex gap-4">
                        <a href="https://github.com/qayasmehtab" target="_blank" class="font-bold text-sm flex items-center text-white">
                            Check README <i class="fa-solid fa-chevron-right ml-2 text-sky-500"></i>
                        </a>
                    </div>
                </div>

                <!-- Project Card 2 -->
                <div class="glass p-8 md:p-12 rounded-[3rem] card-hover group border-l-8 border-indigo-500">
                    <div class="flex justify-between items-start mb-8">
                        <div class="w-12 h-12 bg-indigo-500 rounded-2xl flex items-center justify-center text-white">
                            <i class="fa-solid fa-car text-2xl"></i>
                        </div>
                        <span class="text-[10px] font-black text-indigo-400 bg-indigo-500/10 px-3 py-1 rounded-full uppercase">Automation</span>
                    </div>
                    <h4 class="text-2xl font-black mb-4 group-hover:text-indigo-400 transition">PakWheels Market Scraper</h4>
                    <p class="text-slate-400 mb-8 leading-relaxed">
                        End-to-end scraper using Selenium to track car prices in Pakistan. Automates data collection into structured SQL tables for analysis.
                    </p>
                    <div class="flex gap-4">
                        <a href="https://github.com/qayasmehtab" target="_blank" class="font-bold text-sm flex items-center text-white">
                            View Code <i class="fa-solid fa-chevron-right ml-2 text-indigo-500"></i>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact CTA -->
    <section id="contact" class="py-24 px-6 max-w-5xl mx-auto text-center">
        <div class="glass p-16 rounded-[4rem] relative overflow-hidden border border-sky-500/20 shadow-2xl shadow-sky-500/10">
            <div class="absolute top-0 right-0 w-64 h-64 bg-sky-500/10 rounded-full blur-[100px]"></div>
            <h2 class="text-4xl md:text-6xl font-black mb-8 leading-tight">Ready to optimize your <span class="gradient-text">Data?</span></h2>
            <p class="text-slate-400 text-lg mb-12 max-w-2xl mx-auto font-medium">
                I am actively seeking my first role in Cloud/Data Engineering. Let's discuss how my operational background and technical skills can help your team.
            </p>
            <div class="flex flex-col md:flex-row justify-center items-center gap-6">
                <a href="mailto:qayasabbasi98@gmail.com" class="px-10 py-5 bg-sky-500 rounded-2xl font-black text-white hover:bg-sky-400 transition shadow-lg shadow-sky-500/30 w-full md:w-auto">Hire Qayas Mehtab</a>
                <div class="flex space-x-6">
                    <a href="tel:+923212811321" class="w-14 h-14 bg-white/5 rounded-2xl flex items-center justify-center hover:bg-white/10 transition border border-white/5"><i class="fa-solid fa-phone"></i></a>
                    <a href="https://linkedin.com/in/qayas" class="w-14 h-14 bg-white/5 rounded-2xl flex items-center justify-center hover:bg-white/10 transition border border-white/5"><i class="fa-brands fa-linkedin-in text-sky-400"></i></a>
                </div>
            </div>
        </div>
    </section>

    <footer class="py-12 border-t border-white/5 text-center">
        <p class="text-slate-600 text-xs font-bold uppercase tracking-[0.5em]">2025 | Qayas Mehtab | Architecting Data Flow</p>
    </footer>

</body>
</html>
