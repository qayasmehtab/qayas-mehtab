<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Qayas Mehtab | Cloud Data Engineer Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;900&display=swap');
        
        body { 
            font-family: 'Inter', sans-serif; 
            background-color: #0f172a; 
            color: #f8fafc; 
            scroll-behavior: smooth; 
        }

        .glass { 
            background: rgba(30, 41, 59, 0.7); 
            backdrop-filter: blur(12px); 
            border: 1px solid rgba(255,255,255,0.08); 
        }

        .gradient-text { 
            background: linear-gradient(90deg, #38bdf8, #818cf8); 
            -webkit-background-clip: text; 
            -webkit-text-fill-color: transparent; 
        }

        .card-hover { 
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275); 
        }

        .card-hover:hover { 
            transform: translateY(-12px); 
            border-color: #38bdf8; 
            box-shadow: 0 20px 40px -20px rgba(56, 189, 248, 0.4); 
        }

        .banner-mesh {
            position: absolute;
            top: 0; left: 0; width: 100%; height: 100%;
            background: 
                radial-gradient(circle at 10% 20%, rgba(56, 189, 248, 0.12) 0%, transparent 40%),
                radial-gradient(circle at 90% 80%, rgba(129, 140, 248, 0.12) 0%, transparent 40%);
            z-index: -1;
        }
        
        .floating { animation: float 6s ease-in-out infinite; }
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
        }

        .nav-active { color: #38bdf8; position: relative; }
        .nav-active::after {
            content: '';
            position: absolute;
            bottom: -4px; left: 0; width: 100%; height: 2px;
            background: #38bdf8;
            border-radius: 2px;
        }

        /* Mobile Menu Animation */
        #mobile-menu {
            transition: transform 0.3s ease-in-out;
            transform: translateY(-100%);
        }
        #mobile-menu.active {
            transform: translateY(0);
        }
    </style>
</head>
<body class="selection:bg-sky-500/30">

    <!-- Navbar -->
    <nav class="fixed w-full z-[100] glass border-b border-white/5">
        <div class="max-w-7xl mx-auto px-6 py-4 flex justify-between items-center">
            <a href="#" class="text-2xl font-black tracking-tighter">QAYAS<span class="text-sky-400">.</span>MEHTAB</a>
            
            <!-- Desktop Nav -->
            <div class="hidden md:flex space-x-8 text-[11px] font-bold uppercase tracking-widest items-center">
                <a href="#about" class="hover:text-sky-400 transition-colors">About</a>
                <a href="#skills" class="hover:text-sky-400 transition-colors">Skills</a>
                <a href="#projects" class="hover:text-sky-400 transition-colors">Projects</a>
                <a href="#education" class="hover:text-sky-400 transition-colors">Education</a>
                <a href="#contact" class="bg-sky-500 hover:bg-sky-400 text-white px-5 py-2.5 rounded-xl transition-all shadow-lg shadow-sky-500/20">Hire Me</a>
            </div>

            <!-- Mobile Toggle -->
            <button id="menu-btn" class="md:hidden text-2xl focus:outline-none">
                <i class="fa-solid fa-bars-staggered"></i>
            </button>
        </div>

        <!-- Mobile Menu -->
        <div id="mobile-menu" class="absolute top-0 left-0 w-full glass h-screen flex flex-col items-center justify-center space-y-8 md:hidden -z-10">
            <button id="close-btn" class="absolute top-6 right-6 text-2xl"><i class="fa-solid fa-xmark"></i></button>
            <a href="#about" class="text-2xl font-bold">About</a>
            <a href="#skills" class="text-2xl font-bold">Skills</a>
            <a href="#projects" class="text-2xl font-bold">Projects</a>
            <a href="#education" class="text-2xl font-bold">Education</a>
            <a href="#contact" class="bg-sky-500 px-8 py-3 rounded-2xl font-bold">Hire Me</a>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="relative min-h-screen flex items-center justify-center pt-20 px-6 overflow-hidden">
        <div class="banner-mesh"></div>
        
        <div class="absolute top-1/4 left-10 text-sky-500/5 text-[12rem] font-black select-none floating" style="animation-delay: 1s;">{ }</div>
        <div class="absolute bottom-1/4 right-10 text-indigo-500/5 text-[10rem] font-black select-none floating">DB</div>
        
        <div class="max-w-7xl w-full grid lg:grid-cols-2 gap-16 items-center z-10">
            <div>
                <div class="inline-flex items-center space-x-2 px-3 py-1 rounded-full border border-sky-500/30 bg-sky-500/10 text-sky-400 text-[10px] font-bold mb-8 tracking-[0.2em] uppercase">
                    <span class="relative flex h-2 w-2">
                      <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-sky-400 opacity-75"></span>
                      <span class="relative inline-flex rounded-full h-2 w-2 bg-sky-500"></span>
                    </span>
                    <span>Ready for Entry-Level Cloud Role</span>
                </div>
                <h1 class="text-5xl md:text-7xl lg:text-8xl font-black mb-8 leading-[1]">
                    Cloud <span class="gradient-text">Data</span> <br> Engineer
                </h1>
                <p class="text-slate-400 text-lg md:text-xl mb-10 max-w-xl font-light leading-relaxed">
                    Bridging the gap between <span class="text-white font-semibold">Operational Excellence</span> and <span class="text-white font-semibold">Scalable Data Pipelines</span>. 
                </p>
                <div class="flex flex-wrap gap-4 mb-10">
                    <a href="#projects" class="bg-sky-500 hover:bg-sky-400 text-white px-8 py-4 rounded-2xl font-bold transition-all shadow-xl shadow-sky-500/20 flex items-center group">
                        Explore Work <i class="fa-solid fa-arrow-right ml-2 group-hover:translate-x-1 transition-transform"></i>
                    </a>
                    <a href="mailto:qayasabbasi98@gmail.com" class="glass px-8 py-4 rounded-2xl font-bold hover:bg-white/5 transition-all">Download CV</a>
                </div>
                <div class="flex space-x-6 text-2xl text-slate-500">
                    <a href="https://linkedin.com/in/qayas" target="_blank" class="hover:text-sky-400 transition"><i class="fa-brands fa-linkedin"></i></a>
                    <a href="https://github.com/qayasmehtab" target="_blank" class="hover:text-white transition"><i class="fa-brands fa-github"></i></a>
                </div>
            </div>

            <div class="hidden lg:block relative group">
                <div class="glass p-10 rounded-[3.5rem] border-white/10 shadow-2xl relative z-10 card-hover">
                    <div class="flex items-center space-x-2 mb-8">
                        <div class="w-3 h-3 rounded-full bg-red-500/50"></div>
                        <div class="w-3 h-3 rounded-full bg-yellow-500/50"></div>
                        <div class="w-3 h-3 rounded-full bg-green-500/50"></div>
                    </div>
                    <div class="space-y-6 font-mono text-sm">
                        <div class="p-5 bg-slate-900/80 rounded-2xl border border-white/5">
                            <code class="text-sky-400 italic"># Pipeline status: active</code> <br>
                            <code class="text-emerald-400">extract</code><code class="text-slate-300">(raw_source)</code> <br>
                            <code class="text-emerald-400">transform</code><code class="text-slate-300">(pandas_logic)</code> <br>
                            <code class="text-emerald-400">load</code><code class="text-slate-300">(snowflake_warehouse)</code>
                        </div>
                        <div class="grid grid-cols-2 gap-4">
                            <div class="p-5 bg-sky-500/5 rounded-2xl border border-sky-500/10">
                                <span class="block text-slate-500 text-[10px] uppercase font-bold mb-1">Ops Experience</span>
                                <span class="text-2xl font-black text-white">7+ Years</span>
                            </div>
                            <div class="p-5 bg-indigo-500/5 rounded-2xl border border-indigo-500/10">
                                <span class="block text-slate-500 text-[10px] uppercase font-bold mb-1">Data Quality</span>
                                <span class="text-2xl font-black text-sky-400">99.9%</span>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="absolute -inset-10 bg-sky-500/10 blur-[100px] rounded-full -z-10 group-hover:bg-sky-500/20 transition-all"></div>
            </div>
        </div>
    </section>

    <!-- About / Background Section -->
    <section id="about" class="py-24 px-6 max-w-7xl mx-auto">
        <div class="grid md:grid-cols-12 gap-12 items-start">
            <div class="md:col-span-4">
                <h2 class="text-sm font-black text-sky-400 tracking-[0.3em] uppercase mb-4">The Professional Journey</h2>
                <h3 class="text-4xl font-black text-white leading-tight">From Operations to <span class="gradient-text">Engineering</span></h3>
            </div>
            <div class="md:col-span-8 space-y-8 text-slate-400 text-lg leading-relaxed font-light">
                <p>
                    With over <span class="text-white font-medium">7 years of operational excellence at Air Blue Limited</span>, I have managed large-scale inventory datasets, maintained mission-critical stock reports, and ensured data consistency across cross-functional teams. This background instilled a deep respect for <span class="text-white font-medium">data integrity</span> and process discipline.
                </p>
                <p>
                    Today, I am leveraging that "real-world" experience to build technical solutions. I specialize in Python-based ETL frameworks, web scraping with Selenium, and cloud data warehousing. My goal is to transform complex, raw data into structured assets that drive strategic decision-making.
                </p>
                
                <div class="grid sm:grid-cols-2 gap-6 pt-6">
                    <div class="p-6 rounded-3xl bg-slate-800/30 border border-white/5">
                        <h4 class="text-white font-bold mb-2 flex items-center">
                            <i class="fa-solid fa-plane-up text-sky-400 mr-2 text-sm"></i> Air Blue (2017-2024)
                        </h4>
                        <p class="text-sm">Supervised warehouse data and procurement logs, managing 100k+ inventory units with zero discrepancies.</p>
                    </div>
                    <div class="p-6 rounded-3xl bg-slate-800/30 border border-white/5">
                        <h4 class="text-white font-bold mb-2 flex items-center">
                            <i class="fa-solid fa-headset text-sky-400 mr-2 text-sm"></i> TRG (IBEX Global)
                        </h4>
                        <p class="text-sm">Honed communication and analytical problem-solving skills in high-pressure customer account management.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="py-24 px-6 glass relative">
        <div class="max-w-7xl mx-auto">
            <h3 class="text-center text-sm font-bold text-sky-400 tracking-[0.3em] uppercase mb-16">Core Competencies</h3>
            <div class="grid grid-cols-2 lg:grid-cols-4 gap-8">
                <!-- Python -->
                <div class="p-8 rounded-[2rem] bg-slate-900/50 border border-white/5 card-hover text-center">
                    <div class="w-16 h-16 bg-sky-500/10 rounded-2xl flex items-center justify-center mx-auto mb-6">
                        <i class="fa-brands fa-python text-3xl text-sky-400"></i>
                    </div>
                    <h4 class="font-bold text-xl mb-2">Python Ecosystem</h4>
                    <p class="text-slate-500 text-xs">Pandas, NumPy, Matplotlib, Requests</p>
                </div>
                <!-- Data Engineering -->
                <div class="p-8 rounded-[2rem] bg-slate-900/50 border border-white/5 card-hover text-center">
                    <div class="w-16 h-16 bg-emerald-500/10 rounded-2xl flex items-center justify-center mx-auto mb-6">
                        <i class="fa-solid fa-gears text-3xl text-emerald-400"></i>
                    </div>
                    <h4 class="font-bold text-xl mb-2">ETL Pipelines</h4>
                    <p class="text-slate-500 text-xs">Extraction, Transformation, Loading & Validation</p>
                </div>
                <!-- Databases -->
                <div class="p-8 rounded-[2rem] bg-slate-900/50 border border-white/5 card-hover text-center">
                    <div class="w-16 h-16 bg-indigo-500/10 rounded-2xl flex items-center justify-center mx-auto mb-6">
                        <i class="fa-solid fa-database text-3xl text-indigo-400"></i>
                    </div>
                    <h4 class="font-bold text-xl mb-2">Modern Warehousing</h4>
                    <p class="text-slate-500 text-xs">Snowflake, AWS, SQL Server</p>
                </div>
                <!-- Automation -->
                <div class="p-8 rounded-[2rem] bg-slate-900/50 border border-white/5 card-hover text-center">
                    <div class="w-16 h-16 bg-amber-500/10 rounded-2xl flex items-center justify-center mx-auto mb-6">
                        <i class="fa-solid fa-robot text-3xl text-amber-400"></i>
                    </div>
                    <h4 class="font-bold text-xl mb-2">Web Automation</h4>
                    <p class="text-slate-500 text-xs">Selenium, BS4, Scrapy</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="py-24 px-6 max-w-7xl mx-auto">
        <div class="flex flex-col md:flex-row justify-between items-end mb-16 gap-4">
            <div>
                <h2 class="text-sm font-black text-sky-400 tracking-[0.3em] uppercase mb-4">Portfolio</h2>
                <h3 class="text-5xl font-black text-white">Featured <span class="gradient-text">Builds</span></h3>
            </div>
            <a href="https://github.com/qayasmehtab" target="_blank" class="text-slate-400 hover:text-white transition font-bold flex items-center underline decoration-sky-500/50 underline-offset-8">
                View All Repositories <i class="fa-solid fa-arrow-up-right-from-square ml-2 text-xs"></i>
            </a>
        </div>
        
        <div class="grid lg:grid-cols-3 gap-8">
            <!-- Project 1 -->
            <div class="glass p-8 rounded-[3rem] card-hover relative group border-t-4 border-sky-500">
                <div class="text-[10px] font-black tracking-widest text-sky-400 mb-4 flex justify-between uppercase">
                    <span>Framework</span>
                    <i class="fa-brands fa-github text-lg text-slate-600"></i>
                </div>
                <h4 class="text-2xl font-bold mb-6 text-white">Modular ETL Core</h4>
                <p class="text-slate-400 text-sm leading-relaxed mb-8">
                    A custom-built Python framework featuring advanced logging, automated CSV transformation, and robust SQL injection validation.
                </p>
                <div class="flex flex-wrap gap-2 mb-8">
                    <span class="bg-white/5 px-3 py-1.5 rounded-lg text-[10px] font-bold">LOGGING</span>
                    <span class="bg-white/5 px-3 py-1.5 rounded-lg text-[10px] font-bold">SQL_ENGINE</span>
                </div>
                <a href="https://github.com/qayasmehtab" target="_blank" class="w-full py-4 bg-sky-500/10 hover:bg-sky-500/20 text-sky-400 rounded-2xl text-xs font-bold transition flex items-center justify-center">
                    Source Code <i class="fa-solid fa-code ml-2"></i>
                </a>
            </div>

            <!-- Project 2 -->
            <div class="glass p-8 rounded-[3rem] card-hover relative group border-t-4 border-emerald-500">
                <div class="text-[10px] font-black tracking-widest text-emerald-400 mb-4 flex justify-between uppercase">
                    <span>Automated Pipeline</span>
                    <i class="fa-brands fa-github text-lg text-slate-600"></i>
                </div>
                <h4 class="text-2xl font-bold mb-6 text-white">PakWheels Market Analysis</h4>
                <p class="text-slate-400 text-sm leading-relaxed mb-8">
                    Full-cycle pipeline: Scraping vehicle data via Selenium, cleaning with Pandas, and loading into SQL Server for market valuation.
                </p>
                <div class="flex flex-wrap gap-2 mb-8">
                    <span class="bg-white/5 px-3 py-1.5 rounded-lg text-[10px] font-bold">SELENIUM</span>
                    <span class="bg-white/5 px-3 py-1.5 rounded-lg text-[10px] font-bold">PANDAS</span>
                </div>
                <a href="https://github.com/qayasmehtab" target="_blank" class="w-full py-4 bg-emerald-500/10 hover:bg-emerald-500/20 text-emerald-400 rounded-2xl text-xs font-bold transition flex items-center justify-center">
                    Source Code <i class="fa-solid fa-code ml-2"></i>
                </a>
            </div>

            <!-- Project 3 -->
            <div class="glass p-8 rounded-[3rem] card-hover relative group border-t-4 border-indigo-500">
                <div class="text-[10px] font-black tracking-widest text-indigo-400 mb-4 flex justify-between uppercase">
                    <span>Data Scraping</span>
                    <i class="fa-brands fa-github text-lg text-slate-600"></i>
                </div>
                <h4 class="text-2xl font-bold mb-6 text-white">Banggood Product Scraper</h4>
                <p class="text-slate-400 text-sm leading-relaxed mb-8">
                    Scalable BeautifulSoup-based scraper designed to parse thousands of product listings into structured relational database tables.
                </p>
                <div class="flex flex-wrap gap-2 mb-8">
                    <span class="bg-white/5 px-3 py-1.5 rounded-lg text-[10px] font-bold">BEAUTIFULSOUP</span>
                    <span class="bg-white/5 px-3 py-1.5 rounded-lg text-[10px] font-bold">DATAFRAMES</span>
                </div>
                <a href="https://github.com/qayasmehtab" target="_blank" class="w-full py-4 bg-indigo-500/10 hover:bg-indigo-500/20 text-indigo-400 rounded-2xl text-xs font-bold transition flex items-center justify-center">
                    Source Code <i class="fa-solid fa-code ml-2"></i>
                </a>
            </div>
        </div>
    </section>

    <!-- Education Section -->
    <section id="education" class="py-24 px-6 bg-slate-900/30">
        <div class="max-w-4xl mx-auto">
            <h3 class="text-center text-sm font-black text-sky-400 tracking-[0.3em] uppercase mb-16">Academic Foundation</h3>
            <div class="space-y-12">
                <div class="flex flex-col md:flex-row md:items-center justify-between p-10 glass rounded-[2.5rem] border-white/5 group">
                    <div>
                        <span class="text-sky-400 font-bold text-xs uppercase tracking-widest mb-2 block">Post-Graduation / Ongoing</span>
                        <h4 class="text-2xl font-black text-white">Commerce & Business Studies</h4>
                        <p class="text-slate-400 mt-2">Focused on data-driven business strategy and financial auditing.</p>
                    </div>
                    <div class="mt-6 md:mt-0 text-slate-500 font-mono text-sm border-l md:border-l-0 md:pl-0 pl-6 border-sky-500/30">
                        Higher Education <br> Commission
                    </div>
                </div>
                
                <div class="text-center">
                    <p class="text-slate-500 text-sm">Actively pursuing certifications in <span class="text-sky-400">AWS Cloud Practitioner</span> and <span class="text-sky-400">Snowflake Essentials</span>.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-24 px-6">
        <div class="max-w-5xl mx-auto glass p-16 rounded-[4rem] text-center border border-white/5 relative overflow-hidden">
            <div class="absolute -top-20 -left-20 w-80 h-80 bg-sky-500/5 rounded-full blur-[120px]"></div>
            <div class="absolute -bottom-20 -right-20 w-80 h-80 bg-indigo-500/5 rounded-full blur-[120px]"></div>
            
            <h2 class="text-sm font-black text-sky-400 tracking-[0.4em] uppercase mb-6">Let's Connect</h2>
            <h3 class="text-5xl md:text-6xl font-black mb-10 text-white leading-tight">Ready to build the <br> <span class="gradient-text">Future of Data</span>.</h3>
            
            <p class="text-slate-400 mb-16 text-lg max-w-2xl mx-auto font-light leading-relaxed">
                Currently open to entry-level Cloud or Data Engineering roles. Let's discuss how my operational discipline and technical skills can benefit your team.
            </p>
            
            <div class="grid md:grid-cols-2 gap-6 mb-16">
                <a href="mailto:qayasabbasi98@gmail.com" class="p-8 bg-slate-800/50 rounded-3xl border border-slate-700 hover:border-sky-500 transition-all group flex flex-col items-center">
                    <i class="fa-solid fa-envelope text-sky-400 text-3xl mb-4 group-hover:scale-110 transition-transform"></i>
                    <div class="text-sm font-bold text-white mb-1">qayasabbasi98@gmail.com</div>
                    <div class="text-[10px] text-slate-500 uppercase tracking-widest">Email me anytime</div>
                </a>
                <a href="tel:+923212811321" class="p-8 bg-slate-800/50 rounded-3xl border border-slate-700 hover:border-sky-500 transition-all group flex flex-col items-center">
                    <i class="fa-solid fa-phone text-sky-400 text-3xl mb-4 group-hover:scale-110 transition-transform"></i>
                    <div class="text-sm font-bold text-white mb-1">+92 321 2811321</div>
                    <div class="text-[10px] text-slate-500 uppercase tracking-widest">Mobile / WhatsApp</div>
                </a>
            </div>
            
            <div class="flex justify-center space-x-12">
                <a href="https://linkedin.com/in/qayas" class="text-slate-500 hover:text-sky-400 transition-colors text-4xl" target="_blank"><i class="fa-brands fa-linkedin"></i></a>
                <a href="https://github.com/qayasmehtab" class="text-slate-500 hover:text-white transition-colors text-4xl" target="_blank"><i class="fa-brands fa-github"></i></a>
            </div>
        </div>
    </section>

    <footer class="py-12 text-center text-slate-700 text-[9px] tracking-[0.5em] uppercase border-t border-slate-900/50">
        &copy; 2025 QAYAS MEHTAB | CLOUD DATA ENGINEER | BUILT FOR PERFORMANCE
    </footer>

    <script>
        // Mobile menu logic
        const menuBtn = document.getElementById('menu-btn');
        const closeBtn = document.getElementById('close-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        const mobileLinks = mobileMenu.querySelectorAll('a');

        const toggleMenu = () => {
            mobileMenu.classList.toggle('active');
            document.body.style.overflow = mobileMenu.classList.contains('active') ? 'hidden' : '';
        };

        menuBtn.addEventListener('click', toggleMenu);
        closeBtn.addEventListener('click', toggleMenu);
        mobileLinks.forEach(link => link.addEventListener('click', toggleMenu));

        // Smooth reveal on scroll (simplified)
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('opacity-100', 'translate-y-0');
                    entry.target.classList.remove('opacity-0', 'translate-y-10');
                }
            });
        }, { threshold: 0.1 });

        document.querySelectorAll('section').forEach(section => {
            section.classList.add('transition-all', 'duration-1000', 'opacity-0', 'translate-y-10');
            observer.observe(section);
        });
    </script>
</body>
</html>
