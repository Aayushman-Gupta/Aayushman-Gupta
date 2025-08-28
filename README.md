<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aayushman Gupta</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap');
        body {
            font-family: 'Inter', sans-serif;
            background-color: #0f172a;
            color: #e2e8f0;
            line-height: 1.6;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 2rem;
        }
        .card {
            background-color: #1a202c;
            border-radius: 1.5rem;
            padding: 2rem;
            margin-bottom: 2rem;
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.2), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
        }
        .fade-in {
            opacity: 0;
            animation: fadeInAnimation 1s ease-in forwards;
        }
        @keyframes fadeInAnimation {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .delay-1 { animation-delay: 0.2s; }
        .delay-2 { animation-delay: 0.4s; }
        .delay-3 { animation-delay: 0.6s; }
        .delay-4 { animation-delay: 0.8s; }
        .delay-5 { animation-delay: 1.0s; }
        .icon {
            display: inline-block;
            vertical-align: middle;
            margin-right: 8px;
        }
        .project-card:hover .project-title {
            color: #63b3ed;
        }
        .icon-lg {
            width: 24px;
            height: 24px;
        }
        /* New Animations */
        .profile-pic-pulse {
            animation: pulse-fade 2s infinite ease-in-out;
        }
        @keyframes pulse-fade {
            0% { box-shadow: 0 0 0 0 rgba(100, 116, 139, 0.4); }
            70% { box-shadow: 0 0 0 10px rgba(100, 116, 139, 0); }
            100% { box-shadow: 0 0 0 0 rgba(100, 116, 139, 0); }
        }
        .skill-item {
            transition: transform 0.2s ease;
        }
        .skill-item:hover {
            transform: scale(1.05);
        }
        .connect-link:hover {
            transform: scale(1.05);
            animation: bounce-in 0.5s ease-out;
        }
        @keyframes bounce-in {
            0% { transform: scale(0.9); }
            50% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }
    </style>
</head>
<body>

<div class="container">
    <!-- Header Section -->
    <header class="text-center mb-12 fade-in">
        <div class="w-32 h-32 mx-auto mb-4 rounded-full overflow-hidden border-4 border-gray-600 profile-pic-pulse">
            <img src="https://placehold.co/128x128/334155/e2e8f0?text=AG" alt="Aayushman Gupta" class="w-full h-full object-cover">
        </div>
        <h1 class="text-4xl font-bold text-white mb-2">Aayushman Gupta</h1>
        <h3 class="text-xl text-gray-400 font-semibold">Computer Science Student | Full-Stack Developer | Research Enthusiast</h3>
    </header>

    <!-- About Me Section -->
    <div class="card fade-in delay-1">
        <h2 class="text-2xl font-bold mb-4 flex items-center">
            <svg class="icon icon-lg" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                <path d="M19 21v-2a4 4 0 0 0-4-4H9a4 4 0 0 0-4 4v2"></path>
                <circle cx="12" cy="7" r="4"></circle>
            </svg>
            About Me
        </h2>
        <p class="text-gray-300">
            I'm a B.Tech student in Computer Science and Engineering at IIIT Sonepat, passionate about building scalable full-stack applications and exploring cutting-edge research in computer science. With a strong foundation in data structures, algorithms, and system design, I love tackling complex problems and creating real-world solutions.
        </p>
        <ul class="mt-4 space-y-2 text-gray-400">
            <li>🎓 <span class="font-semibold text-white">Education:</span> Indian Institute of Information Technology (IIIT) Sonepat</li>
            <li>💼 <span class="font-semibold text-white">Experience:</span> I have hands-on experience in full-stack development and research, with a focus on real-time systems, concurrency, and network protocols.</li>
            <li>🏆 <span class="font-semibold text-white">Achievements:</span>
                <ul class="list-disc list-inside ml-4">
                    <li><span class="text-yellow-400">✨</span> Solved 450+ algorithmic problems on platforms like LeetCode and HackerRank, achieving a rating of 1750+.</li>
                    <li><span class="text-yellow-400">✨</span> Ranked 4th in the HackZilla Hackathon, building a full-stack solution in under 24 hours.</li>
                    <li><span class="text-yellow-400">✨</span> 2x Chess Gold Medalist in the intra-college sports championship.</li>
                </ul>
            </li>
        </ul>
    </div>

    <!-- Technical Skills Section -->
    <div class="card fade-in delay-2">
        <h2 class="text-2xl font-bold mb-4 flex items-center">
            <svg class="icon icon-lg" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                <path d="M6 8l-2 5h-2l5 2l-2 5h2l5-2l5 2h2l-2-5l5-2l-2-5h-2l-5 2z"></path>
            </svg>
            Technical Skills
        </h2>
        <div class="grid grid-cols-2 sm:grid-cols-3 gap-4 text-center">
            <div class="p-3 bg-slate-800 rounded-lg skill-item">👨‍💻 C, C++, Java, Python</div>
            <div class="p-3 bg-slate-800 rounded-lg skill-item">🌐 JavaScript, SQL, HTML, CSS</div>
            <div class="p-3 bg-slate-800 rounded-lg skill-item">⚛️ React.js, Django, Node.js</div>
            <div class="p-3 bg-slate-800 rounded-lg skill-item">💾 PostgreSQL, MongoDB, MySQL</div>
            <div class="p-3 bg-slate-800 rounded-lg skill-item">🛠️ Git, GitHub, VS Code</div>
            <div class="p-3 bg-slate-800 rounded-lg skill-item">🧠 DSA, OOP, OS, DBMS</div>
        </div>
    </div>

    <!-- Projects Section -->
    <div class="card fade-in delay-3">
        <h2 class="text-2xl font-bold mb-4 flex items-center">
            <svg class="icon icon-lg" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                <path d="M12 2L2 7l10 5l10-5l-10-5zM2 17l10 5l10-5M2 12l10 5l10-5"></path>
            </svg>
            Projects
        </h2>
        <div class="space-y-6">
            <div class="project-card card bg-gray-800 transition-colors duration-300 hover:bg-gray-700 p-6 rounded-xl">
                <h3 class="text-xl font-semibold mb-2 project-title">🚧 Mela Safe | Real-Time Stampede Prevention System</h3>
                <p class="text-gray-400 text-sm mb-2">**Tech Stack:** Django, React, C++, Python, NumPy</p>
                <p class="text-gray-300">
                    Designed a system to handle 100,000+ individuals by integrating pathfinding algorithms and an LSTM model for crowd movement prediction. The system achieved over 90% temporal accuracy in predicting congestion zones and reduced potential congestion by up to 40% in simulations.
                </p>
            </div>
            <div class="project-card card bg-gray-800 transition-colors duration-300 hover:bg-gray-700 p-6 rounded-xl">
                <h3 class="text-xl font-semibold mb-2 project-title">📈 Multithreaded Stock Price Simulator | C++, Concurrency</h3>
                <p class="text-gray-400 text-sm mb-2">**Tech Stack:** C++, Concurrency, Producer-Consumer</p>
                <p class="text-gray-300">
                    Spearheaded a producer-consumer based simulator where multiple threads generate and process live stock price updates in real-time. The system was architected with a thread-safe queue, achieving 100% race-free execution and a 40% performance improvement over naive synchronization methods.
                </p>
            </div>
            <div class="project-card card bg-gray-800 transition-colors duration-300 hover:bg-gray-700 p-6 rounded-xl">
                <h3 class="text-xl font-semibold mb-2 project-title">🛒 TrainMe | Full-Stack Course Selling Platform</h3>
                <p class="text-gray-400 text-sm mb-2">**Tech Stack:** React, Django, PostgreSQL</p>
                <p class="text-gray-300">
                    Developed a scalable platform supporting over 1000 concurrent users. Implemented real-time filtering and keyword-based search that improved course discovery by 60%, and managed over 10K user-course records with a normalized database schema.
                </p>
            </div>
        </div>
    </div>

    <!-- Contact Section -->
    <div class="card text-center fade-in delay-5">
        <h2 class="text-2xl font-bold mb-4">Let's Connect!</h2>
        <div class="flex justify-center space-x-4">
            <a href="https://www.linkedin.com/in/aayushman-gupta-28b2a2291/" target="_blank" rel="noopener noreferrer" class="connect-link">
                <img src="https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin" alt="LinkedIn" />
            </a>
            <a href="mailto:aayushmangupta780@gmail.com" class="connect-link">
                <img src="https://img.shields.io/badge/Gmail-red?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
            </a>
        </div>
    </div>
</div>

</body>
</html>

