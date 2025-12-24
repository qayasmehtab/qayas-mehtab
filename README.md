<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Qayas Mehtab | Cloud Data Engineer Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap');
        body { font-family: 'Inter', sans-serif; background-color: #0f172a; color: #f8fafc; scroll-behavior: smooth; }
        .glass { background: rgba(30, 41, 59, 0.7); backdrop-filter: blur(10px); border: 1px solid rgba(255,255,255,0.1); }
        .gradient-text { background: linear-gradient(90deg, #38bdf8, #818cf8); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }
        .card-hover { transition: all 0.3s ease; }
        .card-hover:hover { transform: translateY(-8px); border-color: #38bdf8; box-shadow: 0 10px 30px -10px rgba(56, 189, 248, 0.3); }
        .nav-link:hover { color: #38bdf8; text-shadow: 0 0 10px rgba(56, 189, 248, 0.5); }
        
        /* Animated Background for Banner */
        .banner-mesh {
            position: absolute;
            top: 0; left: 0; width: 100%; height: 100%;
            background: radial-gradient(circle at 20% 30%, rgba(56, 189, 248, 0.15) 0%, transparent 50%),
                        radial-gradient(circle at 80% 70%, rgba(129, 140, 248, 0.15) 0%, transparent 50%);
            z-index: -1;
        }
        
        .floating {
            animation: float 6s ease-in-out infinite;
        }
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
            100% { transform: translateY(0px); }
        }
    </style>
</head>
<body>

    <!-- Navbar -->
    <nav class="fixed w-full z-50 glass">
        <div class="max-w-6xl mx-auto px-6 py-4 flex justify-between items-center">
            <a href="#" class="text-2xl font-bold tracking-tighter">QAYAS<span class="text-sky-400">.</span>MEHTAB</a>
            <div class="hidden md:flex space-x-8 text-xs font-bold uppercase tracking-widest items-center">
                <a href="#about" class="nav-link">About</a>
                <a href="#skills" class="nav-link">Skills</a>
                <a href="#projects" class="nav-link">Projects</a>
                <a href="#contact" class="nav-link bg-sky-500/10 px-4 py-2 rounded-lg border border-sky-500/20">Hire Me</a>
            </div>
        </div>
    </nav>

    <!-- Main Banner Section -->
    <section class="relative min-h-screen flex items-center justify-center pt-20 px-6 overflow-hidden">
        <div class="banner-mesh"></div>
        
        <!-- Background Data Symbols -->
        <div class="absolute top-1/4 left-10 text-sky-500/10 text-9xl font-bold select-none floating" style="animation-delay: 1s;">{ }</div>
        <div class="absolute bottom-1/4 right-10 text-indigo-500/10 text-9xl font-bold select-none floating">SQL</div>
        
        <div class="max-w-6xl w-full grid lg:grid-cols-2 gap-12 items-center z-10">
            <!-- Left Side: Text Content -->
            <div class="text-center lg:text-left">
                <div class="inline-flex items-center space-x-2 px-3 py-1 rounded-full border border-sky-500/30 bg-sky-500/10 text-sky-400 text-[10px] font-bold mb-6 tracking-[0.2em] uppercase">
                    <span class="relative flex h-2 w-2">
                      <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-sky-400 opacity-75"></span>
                      <span class="relative inline-flex rounded-full h-2 w-2 bg-sky-500"></span>
                    </span>
                    <span>Ready for Hire</span>
                </div>
                <h1 class="text-5xl md:text-7xl lg:text-8xl font-black mb-6 leading-[1.1]">
                    Cloud <span class="gradient-text">Data</span> <br> Engineer
                </h1>
                <p class="text-slate-400 text-lg md:text-xl mb-10 max-w-xl font-light leading-relaxed">
                    Transitioning from <span class="text-white font-semibold">7 years of Ops Excellence</span> at Air Blue to building scalable, automated ETL pipelines and data warehouses.
                </p>
                <div class="flex flex-wrap justify-center lg:justify-start gap-4 mb-8">
                    <a href="#projects" class="bg-sky-500 hover:bg-sky-400 text-white px-8 py-4 rounded-2xl font-bold transition-all shadow-xl shadow-sky-500/20 flex items-center group">
                        View Repositories <i class="fa-solid fa-arrow-right ml-2 group-hover:translate-x-1 transition-transform"></i>
                    </a>
                    <a href="#contact" class="glass px-8 py-4 rounded-2xl font-bold hover:bg-white/5 transition-all">Let's Talk</a>
                </div>
                <div class="flex justify-center lg:justify-start space-x-6 text-2xl text-slate-500">
                    <a href="https://linkedin.com/in/qayas" target="_blank" class="hover:text-sky-400 transition"><i class="fa-brands fa-linkedin"></i></a>
                    <a href="https://github.com/qayasmehtab" target="_blank" class="hover:text-white transition"><i class="fa-brands fa-github"></i></a>
                </div>
            </div>

            <!-- Right Side: Visual Element (Data Card) -->
            <div class="hidden lg:block relative floating">
                <div class="glass p-8 rounded-[3rem] border-white/10 shadow-2xl relative z-10">
                    <div class="flex items-center space-x-3 mb-6">
                        <div class="w-3 h-3 rounded-full bg-red-500"></div>
                        <div class="w-3 h-3 rounded-full bg-yellow-500"></div>
                        <div class="w-3 h-3 rounded-full bg-green-500"></div>
                    </div>
                    <div class="space-y-4 font-mono text-sm">
                        <p class="text-sky-400 uppercase text-[10px] font-bold tracking-widest">Incoming Data Pipeline</p>
                        <div class="p-4 bg-slate-900/50 rounded-xl border border-white/5">
                            <code class="text-emerald-400">SELECT</code> <code class="text-slate-300">insights</code> <br>
                            <code class="text-emerald-400">FROM</code> <code class="text-slate-300">raw_web_data</code> <br>
                            <code class="text-emerald-400">WHERE</code> <code class="text-slate-300">status = 'active'</code>
                        </div>
                        <div class="grid grid-cols-2 gap-4">
                            <div class="p-4 bg-slate-900/50 rounded-xl border border-white/5">
                                <span class="block text-slate-500 text-[10px] mb-1">Rows Processed</span>
                                <span class="text-xl font-bold text-white">100K+</span>
                            </div>
                            <div class="p-4 bg-slate-900/50 rounded-xl border border-white/5">
                                <span class="block text-slate-500 text-[10px] mb-1">Integrity</span>
                                <span class="text-xl font-bold text-sky-400">99.9%</span>
                            </div>
                        </div>
                    </div>
                </div>
                <!-- Glowing Orb behind card -->
                <div class="absolute -inset-4 bg-sky-500/20 blur-3xl rounded-full z-0"></div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="py-24 px-6 max-w-6xl mx-auto border-t border-slate-800/50">
        <h3 class="text-center text-sm font-bold text-sky-400 tracking-[0.3em] uppercase mb-16">Tech Stack & Competencies</h3>
        <div class="grid grid-cols-2 md:grid-cols-4 gap-8">
            <div class="glass p-8 rounded-3xl card-hover flex flex-col items-center">
                <div class="w-16 h-16 bg-sky-500/10 rounded-2xl flex items-center justify-center mb-6">
                    <i class="fa-brands fa-python text-3xl text-sky-400"></i>
                </div>
                <h4 class="font-bold text-lg">Python</h4>
                <p class="text-slate-500 text-xs mt-2 text-center">Numpy, Pandas, Matplotlib</p>
            </div>
            <div class="glass p-8 rounded-3xl card-hover flex flex-col items-center">
                <div class="w-16 h-16 bg-sky-500/10 rounded-2xl flex items-center justify-center mb-6">
                    <i class="fa-solid fa-cloud text-3xl text-sky-400"></i>
                </div>
                <h4 class="font-bold text-lg">Cloud/Warehouse</h4>
                <p class="text-slate-500 text-xs mt-2 text-center">Snowflake, AWS, SQL Server</p>
            </div>
            <div class="glass p-8 rounded-3xl card-hover flex flex-col items-center">
                <div class="w-16 h-16 bg-sky-500/10 rounded-2xl flex items-center justify-center mb-6">
                    <i class="fa-solid fa-spider text-3xl text-sky-400"></i>
                </div>
                <h4 class="font-bold text-lg">Web Scraping</h4>
                <p class="text-slate-500 text-xs mt-2 text-center">Selenium, BeautifulSoup</p>
            </div>
            <div class="glass p-8 rounded-3xl card-hover flex flex-col items-center">
                <div class="w-16 h-16 bg-sky-500/10 rounded-2xl flex items-center justify-center mb-6">
                    <i class="fa-solid fa-code-merge text-3xl text-sky-400"></i>
                </div>
                <h4 class="font-bold text-lg">ETL Logic</h4>
                <p class="text-slate-500 text-xs mt-2 text-center">GitBash, Automation, Validation</p>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="py-24 px-6 max-w-7xl mx-auto">
        <h3 class="text-4xl font-black mb-16 text-center text-white uppercase tracking-tighter">My <span class="text-sky-400">Repositories</span></h3>
        
        <div class="grid lg:grid-cols-3 gap-10">
            
            <!-- Project 1: ETL CORE -->
            <div class="glass p-8 rounded-[2.5rem] card-hover relative group border-t-4 border-emerald-500">
                <div class="absolute -top-4 -right-4 bg-emerald-500 text-white text-[10px] font-black px-4 py-2 rounded-xl shadow-lg">GITHUB SOURCE</div>
                <h4 class="text-2xl font-bold mb-6 text-white">Python ETL Framework</h4>
                <div class="space-y-4 mb-8">
                    <div class="flex items-center text-sm text-slate-400">
                        <span class="w-2 h-2 rounded-full bg-emerald-500 mr-3"></span> Modular Logging Functions
                    </div>
                    <div class="flex items-center text-sm text-slate-400">
                        <span class="w-2 h-2 rounded-full bg-emerald-500 mr-3"></span> Robust Data Extraction
                    </div>
                    <div class="flex items-center text-sm text-slate-400">
                        <span class="w-2 h-2 rounded-full bg-emerald-500 mr-3"></span> Database Loading Scripts
                    </div>
                    <div class="flex items-center text-sm text-slate-400">
                        <span class="w-2 h-2 rounded-full bg-emerald-500 mr-3"></span> Log Verification Logic
                    </div>
                </div>
                <div class="flex flex-col gap-4">
                    <a href="https://github.com/qayasmehtab" target="_blank" class="w-full text-center py-3 bg-white/5 hover:bg-white/10 rounded-xl text-xs font-bold transition border border-white/10">View Code on GitHub</a>
                </div>
            </div>

            <!-- Project 2: PakWheels -->
            <div class="glass p-8 rounded-[2.5rem] card-hover border-t-4 border-sky-500">
                <div class="flex justify-between items-center mb-6">
                    <h4 class="text-2xl font-bold text-white">PakWheels Pipeline</h4>
                    <i class="fa-brands fa-github text-2xl text-slate-500"></i>
                </div>
                <p class="text-slate-400 text-sm leading-relaxed mb-8">
                    An automated scraper and ETL tool for vehicle market analysis. Features data cleaning with Pandas and SQL Server integration.
                </p>
                <div class="flex flex-wrap gap-2 mb-8">
                    <span class="bg-sky-500/10 text-sky-400 px-3 py-1 rounded-md text-[10px] font-bold">PYTHON</span>
                    <span class="bg-sky-500/10 text-sky-400 px-3 py-1 rounded-md text-[10px] font-bold">SELENIUM</span>
                </div>
                <a href="https://github.com/qayasmehtab" target="_blank" class="text-sky-400 font-bold text-sm flex items-center group-hover:underline">
                    Read README.md <i class="fa-solid fa-arrow-right ml-2 text-xs"></i>
                </a>
            </div>

            <!-- Project 3: Banggood -->
            <div class="glass p-8 rounded-[2.5rem] card-hover border-t-4 border-indigo-500">
                <div class="flex justify-between items-center mb-6">
                    <h4 class="text-2xl font-bold text-white">Banggood Scraper</h4>
                    <i class="fa-brands fa-github text-2xl text-slate-500"></i>
                </div>
                <p class="text-slate-400 text-sm leading-relaxed mb-8">
                    Large-scale product data acquisition framework. Handles multiple categories and converts HTML into structured SQL tables.
                </p>
                <div class="flex flex-wrap gap-2 mb-8">
                    <span class="bg-indigo-500/10 text-indigo-400 px-3 py-1 rounded-md text-[10px] font-bold">BS4</span>
                    <span class="bg-indigo-500/10 text-indigo-400 px-3 py-1 rounded-md text-[10px] font-bold">SQL SERVER</span>
                </div>
                <a href="https://github.com/qayasmehtab" target="_blank" class="text-indigo-400 font-bold text-sm flex items-center">
                    Check Documentation <i class="fa-solid fa-arrow-right ml-2 text-xs"></i>
                </a>
            </div>

        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-24 px-6">
        <div class="max-w-4xl mx-auto glass p-12 rounded-[3rem] text-center border border-white/5 relative overflow-hidden">
            <div class="absolute -top-10 -left-10 w-40 h-40 bg-sky-500/10 rounded-full blur-2xl"></div>
            <h3 class="text-4xl font-bold mb-8">Let's build the <span class="text-sky-400">Future</span> of Data.</h3>
            <p class="text-slate-400 mb-12 text-lg">Looking for my first role as a Data Engineer. Ready to bring operational discipline to tech.</p>
            
            <div class="grid md:grid-cols-2 gap-8 mb-12">
                <a href="mailto:qayasabbasi98@gmail.com" class="p-6 bg-slate-800/50 rounded-2xl border border-slate-700 hover:border-sky-500 transition">
                    <i class="fa-solid fa-envelope text-sky-400 text-2xl mb-3"></i>
                    <div class="text-sm font-bold">qayasabbasi98@gmail.com</div>
                </a>
                <a href="tel:+923212811321" class="p-6 bg-slate-800/50 rounded-2xl border border-slate-700 hover:border-sky-500 transition">
                    <i class="fa-solid fa-phone text-sky-400 text-2xl mb-3"></i>
                    <div class="text-sm font-bold">+92 321 2811321</div>
                </a>
            </div>
            
            <div class="flex justify-center space-x-8">
                <a href="https://linkedin.com/in/qayas" class="text-slate-500 hover:text-sky-400 transition text-3xl" target="_blank"><i class="fa-brands fa-linkedin"></i></a>
                <a href="https://github.com/qayasmehtab" class="text-slate-500 hover:text-white transition text-3xl" target="_blank"><i class="fa-brands fa-github"></i></a>
            </div>
        </div>
    </section>

    <footer class="py-12 text-center text-slate-600 text-[10px] tracking-[0.4em] uppercase border-t border-slate-900">
        &copy; 2025 QAYAS MEHTAB $|$ DESIGNED FOR HIGH IMPACT
    </footer>

</body>
</html>
