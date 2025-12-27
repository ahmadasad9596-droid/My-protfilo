<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Asad Ahmad | Web Developer & Digital Architect</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;700;800&display=swap');
        body { background-color: #020617; color: white; font-family: 'Plus Jakarta Sans', sans-serif; overflow-x: hidden; scroll-behavior: smooth; }
        .bg-glow { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle at 50% 50%, #1e293b 0%, #020617 100%); z-index: -1; }
        .glass { background: rgba(255, 255, 255, 0.03); backdrop-filter: blur(12px); border: 1px solid rgba(255, 255, 255, 0.08); }
        .text-gradient { background: linear-gradient(90deg, #38bdf8, #818cf8, #c084fc); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }
        #codeModal { display: none; position: fixed; inset: 0; z-index: 1000; background: rgba(2, 6, 23, 0.98); padding: 20px; align-items: center; justify-content: center; }
        .code-box { background: #0f172a; color: #38bdf8; padding: 25px; border-radius: 20px; border: 1px solid #1e293b; font-family: monospace; max-height: 70vh; overflow-y: auto; white-space: pre-wrap; }
    </style>
</head>
<body>
    <div class="bg-glow"></div>

    <div id="codeModal">
        <div class="max-w-4xl w-full p-6">
            <div class="flex justify-between items-center mb-6">
                <h3 class="text-2xl font-bold italic text-sky-400">Neon Trails Source Code</h3>
                <button onclick="closeCode()" class="bg-red-500/20 text-red-500 px-6 py-2 rounded-full font-bold">CLOSE ×</button>
            </div>
            <div class="code-box text-sm md:text-base">
// ASAD AHMAD - Gesture Tracking Logic (Neon Trails)
const isThumbUp = thumbTip.y < thumbIp.y && indexTip.y > indexMcp.y;
if (isThumbUp) {
    trailPoints = []; // Screen Cleared!
    document.getElementById('status').innerText = "CLEARED! ✨";
} else {
    trailPoints.push(new THREE.Vector3(hx, hy, 0));
}
            </div>
        </div>
    </div>

    <nav class="max-w-6xl mx-auto p-8 flex justify-between items-center sticky top-0 z-50 bg-[#020617]/80 backdrop-blur-md">
        <div class="text-2xl font-black italic tracking-tighter">ASAD<span class="text-sky-500">.</span></div>
        <div class="flex gap-6 text-[10px] font-black tracking-widest uppercase text-gray-400">
            <a href="#about" class="hover:text-white transition">About</a>
            <a href="#projects" class="hover:text-white transition">Work</a>
            <a href="#contact" class="text-sky-400 border border-sky-400/30 px-4 py-2 rounded-full hover:bg-sky-400 hover:text-white transition">Hire Me</a>
        </div>
    </nav>

    <section class="min-h-[80vh] flex flex-col items-center justify-center text-center px-6">
        <div data-aos="fade-down" class="mb-6 px-4 py-1 border border-sky-500/20 rounded-full text-sky-400 text-[10px] font-bold tracking-widest bg-sky-500/5 uppercase">Jamia Salafiya, Varanasi</div>
        <h1 data-aos="zoom-in" class="text-6xl md:text-8xl font-black mb-8 tracking-tighter italic text-white">Digital <span class="text-gradient">Architect.</span></h1>
        <p data-aos="fade-up" class="text-gray-400 text-lg md:text-xl max-w-2xl leading-relaxed italic">I turn complex code into interactive experiences. From AI hand-tracking to modern UI, I build the future.</p>
        <div data-aos="fade-up" data-aos-delay="200" class="mt-12 flex flex-wrap justify-center gap-4">
            <a href="#projects" class="bg-sky-500 hover:bg-sky-400 text-white font-black px-10 py-5 rounded-2xl transition shadow-2xl shadow-sky-500/30 uppercase tracking-widest text-xs">View My Work</a>
            <a href="https://instagram.com/_a4asd__" target="_blank" class="glass px-10 py-5 rounded-2xl uppercase tracking-widest text-xs font-black">Instagram</a>
        </div>
    </section>

    <section id="about" class="max-w-6xl mx-auto py-32 px-6">
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-20">
            <div data-aos="fade-right">
                <h2 class="text-sky-500 font-bold tracking-widest text-xs mb-4 uppercase italic">// About Me</h2>
                <h3 class="text-4xl font-extrabold mb-8 leading-tight">Passionate Learner & <span class="text-white">Aspiring Web Developer.</span></h3>
                <div class="text-gray-400 space-y-6 text-lg">
                    <p>I am <span class="text-white font-bold">Asad Ahmad</span>, currently studying at <span class="text-sky-400 font-medium">Jamia Salafiya, Varanasi</span>. My journey is fueled by a problem-solving mindset—breaking complex challenges into simple, logical steps.</p>
                    <p>I enjoy creating interactive websites, experimenting with UI/UX, and understanding how things work behind the scenes. My goal is continuous improvement and ethical work.</p>
                </div>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6" data-aos="fade-left">
                <div class="glass p-8 rounded-[2rem] border-l-4 border-sky-500"><h4 class="text-white font-bold text-xl mb-2">Web Dev</h4><p class="text-gray-500 text-sm">HTML, CSS, JavaScript</p></div>
                <div class="glass p-8 rounded-[2rem] border-l-4 border-purple-500"><h4 class="text-white font-bold text-xl mb-2">Creative AI</h4><p class="text-gray-400 text-sm">Three.js & MediaPipe</p></div>
            </div>
        </div>
    </section>

    <section id="projects" class="max-w-6xl mx-auto py-24 px-6">
        <h2 class="text-3xl font-black mb-16 uppercase italic tracking-widest text-sky-500 underline decoration-sky-500/20">Selected Projects</h2>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-12">
            <div data-aos="fade-up" class="glass p-10 rounded-[3rem] transition-all duration-500 group">
                <div class="flex justify-between items-center mb-6 text-sky-400"><span class="text-[10px] font-black uppercase tracking-[0.3em]">AI Experience</span><i class="fas fa-magic"></i></div>
                <h3 class="text-3xl font-bold mb-4">Neon Trails AI</h3>
                <p class="text-gray-400 mb-8 text-sm">MediaPipe AI tracking ko Three.js engine ke saath merge karke drawing tool banana. "Thumb Reset" logic included.</p>
                <button onclick="openCode()" class="w-full bg-white text-black text-[10px] font-black py-4 rounded-xl uppercase tracking-widest hover:bg-sky-400 hover:text-white transition">View Logic Code</button>
            </div>
            <div data-aos="fade-up" data-aos-delay="200" class="glass p-10 rounded-[3rem] transition-all duration-500">
                <div class="flex justify-between items-center mb-6 text-purple-400"><span class="text-[10px] font-black uppercase tracking-[0.3em]">Utility App</span><i class="fas fa-calculator"></i></div>
                <h3 class="text-3xl font-bold mb-4">Modern Calculator</h3>
                <p class="text-gray-400 mb-8 text-sm">Core JavaScript logic aur modern UI design. Hosted on Netlify.</p>
                <a href="https://peppy-tulumba-fb359a.netlify.app" target="_blank" class="block w-full text-center border border-purple-500 text-purple-400 text-[10px] font-black py-4 rounded-xl uppercase tracking-widest hover:bg-purple-500 hover:text-white transition">Live Demo</a>
            </div>
        </div>
    </section>

    <section id="contact" class="max-w-4xl mx-auto py-32 px-6">
        <div data-aos="zoom-in" class="glass p-12 rounded-[3.5rem]">
            <h2 class="text-5xl font-black mb-12 text-center italic tracking-tighter">Let's <span class="text-gradient">Work.</span></h2>
            <form action="https://formspree.io/f/Ahmadasad9596@gmail.com" method="POST" class="space-y-4">
                <input type="text" name="name" placeholder="Name" class="w-full p-4 rounded-xl bg-white/5 border border-white/10 outline-none focus:border-sky-500 transition" required>
                <input type="email" name="email" placeholder="Email" class="w-full p-4 rounded-xl bg-white/5 border border-white/10 outline-none focus:border-sky-500 transition" required>
                <textarea name="message" rows="4" placeholder="Your Message..." class="w-full p-4 rounded-xl bg-white/5 border border-white/10 outline-none focus:border-sky-500 transition" required></textarea>
                <button type="submit" class="w-full bg-sky-500 text-white font-black py-5 rounded-xl uppercase text-xs tracking-[0.3em] hover:bg-sky-400 transition">Send Message</button>
            </form>
        </div>
    </section>

    <footer class="py-12 text-center text-gray-700 text-[10px] tracking-[0.4em] uppercase">Built by Asad Ahmad © 2025</footer>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });
        function openCode() { document.getElementById('codeModal').style.display = 'flex'; document.body.style.overflow = 'hidden'; }
        function closeCode() { document.getElementById('codeModal').style.display = 'none'; document.body.style.overflow = 'auto'; }
    </script>
</body>
</html>
