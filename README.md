<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AWS x MVJCE | Cloud Horizon</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;700;900&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #0f172a;
            color: white;
            overflow-x: hidden;
        }

        .gradient-bg {
            background: radial-gradient(circle at top right, #2563eb, transparent),
                        radial-gradient(circle at bottom left, #7c3aed, transparent);
        }

        .glass {
            background: rgba(255, 255, 255, 0.03);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.4s ease;
        }

        .glass:hover {
            border: 1px solid rgba(59, 130, 246, 0.5);
            transform: translateY(-5px);
        }

        .hero-text {
            background: linear-gradient(to right, #60a5fa, #a78bfa);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
            100% { transform: translateY(0px); }
        }

        .floating {
            animation: float 6s ease-in-out infinite;
        }

        .aws-orange {
            color: #FF9900;
        }
    </style>
</head>
<body class="gradient-bg min-h-screen">

    <!-- Navigation -->
    <nav class="flex justify-between items-center px-8 py-6 max-w-7xl mx-auto">
        <div class="text-2xl font-black tracking-tighter">
            <span class="aws-orange">AWS</span> <span class="text-slate-400">|</span> MVJCE
        </div>
        <div class="space-x-8 text-sm font-medium hidden md:block">
            <a href="#" class="hover:text-blue-400 transition">Cloud Services</a>
            <a href="#" class="hover:text-blue-400 transition">Student Lab</a>
            <a href="#" class="hover:text-blue-400 transition">Innovation</a>
            <a href="#" class="bg-blue-600 px-5 py-2 rounded-full hover:bg-blue-500 transition">Get Started</a>
        </div>
    </nav>

    <!-- Hero Section -->
    <main class="max-w-7xl mx-auto px-8 pt-20 pb-32 grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
        <div>
            <h1 class="text-7xl md:text-8xl font-black leading-none mb-6">
                AWS <br>
                <span class="hero-text">EVOLUTION.</span>
            </h1>
            <p class="text-xl text-slate-400 mb-10 max-w-md leading-relaxed">
                Empowering the next generation of engineers at <span class="text-white font-bold">MVJ College of Engineering</span>. Scalable infrastructure meets academic excellence.
            </p>
            <div class="flex space-x-4">
                <button class="bg-white text-black px-8 py-4 rounded-xl font-bold hover:bg-slate-200 transition-all">
                    Explore Console
                </button>
                <button class="glass px-8 py-4 rounded-xl font-bold hover:bg-white/10 transition-all">
                    View Projects
                </button>
            </div>
        </div>

        <!-- Decorative Card -->
        <div class="relative py-10">
            <div class="glass p-8 rounded-3xl floating relative z-10">
                <div class="flex justify-between items-start mb-12">
                    <div class="h-12 w-12 bg-blue-500 rounded-lg flex items-center justify-center">
                        <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path></svg>
                    </div>
                    <span class="text-xs font-mono text-slate-500">REGION: MVJCE-SOUTH-1</span>
                </div>
                <h3 class="text-2xl font-bold mb-2">Cloud Computing Lab</h3>
                <p class="text-slate-400 text-sm mb-6">Active instances: 124 <br> Success Rate: 99.9%</p>
                <div class="w-full bg-slate-800 h-2 rounded-full overflow-hidden">
                    <div class="bg-blue-500 h-full w-3/4"></div>
                </div>
            </div>
            <!-- Background Glow -->
            <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-64 h-64 bg-blue-600/30 blur-[100px]"></div>
        </div>
    </main>

    <!-- Stats Section -->
    <section class="max-w-7xl mx-auto px-8 grid grid-cols-2 md:grid-cols-4 gap-6 pb-20">
        <div class="glass p-6 rounded-2xl text-center">
            <div class="text-3xl font-bold mb-1">200+</div>
            <div class="text-xs text-slate-500 uppercase tracking-widest">AWS Services</div>
        </div>
        <div class="glass p-6 rounded-2xl text-center">
            <div class="text-3xl font-bold mb-1">5000+</div>
            <div class="text-xs text-slate-500 uppercase tracking-widest">MVJ Students</div>
        </div>
        <div class="glass p-6 rounded-2xl text-center">
            <div class="text-3xl font-bold mb-1">0.1ms</div>
            <div class="text-xs text-slate-500 uppercase tracking-widest">Latency</div>
        </div>
        <div class="glass p-6 rounded-2xl text-center">
            <div class="text-3xl font-bold mb-1">Infinite</div>
            <div class="text-xs text-slate-500 uppercase tracking-widest">Possibilities</div>
        </div>
    </section>

</body>
</html>
