# projeto-agrinho

projeto feito para concurso agrimho
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu Projeto Avançado | GitHub Pages</title>
    <meta name="description" content="Uma página moderna, responsiva e performática criada para o GitHub.">
    
    <script src="https://cdn.tailwindcss.com"></script>
    
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        brand: {
                            50: '#f0fdf4',
                            500: '#22c55e',
                            600: '#16a34a',
                            900: '#14532d',
                        }
                    }
                }
            }
        }
    </script>

    <style>
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .animate-fade-in {
            animation: fadeIn 0.8s ease-out forwards;
        }
        html {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-gray-50 text-gray-800 dark:bg-gray-950 dark:text-gray-100 transition-colors duration-300 font-sans antialiased">

    <header class="sticky top-0 z-50 backdrop-blur-md bg-white/70 dark:bg-gray-950/70 border-b border-gray-200 dark:border-gray-800 transition-colors">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-16 flex items-center justify-between">
            <div class="flex items-center gap-2">
                <span class="text-xl font-bold bg-gradient-to-r from-brand-600 to-emerald-500 bg-clip-text text-transparent">
                    DevProject
                </span>
            </div>
            
            <nav class="hidden md:flex items-center gap-6 text-sm font-medium">
                <a href="#inicio" class="hover:text-brand-500 transition">Início</a>
                <a href="#recursos" class="hover:text-brand-500 transition">Recursos</a>
                <a href="#sobre" class="hover:text-brand-500 transition">Sobre</a>
                <a href="#contato" class="hover:text-brand-500 transition">Contato</a>
            </nav>

            <div class="flex items-center gap-4">
                <button id="theme-toggle" class="p-2 rounded-lg bg-gray-100 dark:bg-gray-800 hover:ring-2 hover:ring-gray-300 dark:hover:ring-gray-700 transition" aria-label="Alternar tema">
                    <svg id="theme-toggle-dark-icon" class="hidden w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M17.293 13.293A8 8 0 016.707 2.707a8.001 8.001 0 1010.586 10.586z"></path></svg>
                    <svg id="theme-toggle-light-icon" class="hidden w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M10 2a1 1 0 011 1v1a1 1 0 11-2 0V3a1 1 0 011-1zm4 8a4 4 0 11-8 0 4 4 0 018 0zm-.464 4.95l.707.707a1 1 0 001.414-1.414l-.707-.707a1 1 0 00-1.414 1.414zm2.12-10.607a1 1 0 010 1.414l-.706.707a1 1 0 11-1.414-1.414l.707-.707a1 1 0 011.414 0zM17 11a1 1 0 100-2h-1a1 1 0 100 2h1zm-7 4a1 1 0 011 1v1a1 1 0 11-2 0v-1a1 1 0 011-1zM5.05 6.464A1 1 0 106.465 5.05l-.708-.707a1 1 0 00-1.414 1.414l.707.707zm1.414 8.486l-.707.707a1 1 0 01-1.414-1.414l.707-.707a1 1 0 011.414 1.414zM4 11a1 1 0 100-2H3a1 1 0 100 2h1z" fill-rule="evenodd" clip-rule="evenodd"></path></svg>
                </button>
                <a href="https://github.com" target="_blank" class="bg-gray-900 text-white dark:bg-white dark:text-gray-900 px-4 py-2 rounded-lg text-sm font-medium hover:opacity-90 transition">
                    Ver no GitHub
                </a>
            </div>
        </div>
    </header>

    <section id="inicio" class="relative overflow-hidden py-20 lg:py-32">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10 animate-fade-in">
            <div class="text-center max-w-3xl mx-auto">
                <span class="px-3 py-1 text-xs font-semibold bg-brand-50 text-brand-600 dark:bg-brand-900/30 dark:text-brand-500 rounded-full">
                    Deploy Automático via GitHub Actions
                </span>
                <h1 class="mt-6 text-4xl sm:text-6xl font-extrabold tracking-tight text-gray-900 dark:text-white">
                    Uma Interface Avançada para seu <span class="bg-gradient-to-r from-brand-500 to-emerald-400 bg-clip-text text-transparent">Repositório</span>
                </h1>
                <p class="mt-6 text-lg text-gray-600 dark:text-gray-400 structural-fluid">
                    Pronto para produção, otimizado para SEO e construído com ferramentas modernas diretamente no navegador. Modifique e publique instantaneamente.
                </p>
                <div class="mt-10 flex flex-wrap justify-center gap-4">
                    <a href="#recursos" class="bg-brand-600 hover:bg-brand-700 text-white px-6 py-3 rounded-xl font-medium shadow-lg shadow-brand-600/20 transition">
                        Começar Agora
                    </a>
                    <a href="#sobre" class="bg-white text-gray-900 border border-gray-300 dark:bg-gray-900 dark:text-gray-100 dark:border-gray-700 px-6 py-3 rounded-xl font-medium hover:bg-gray-50 dark:hover:bg-gray-800 transition">
                        Saber Mais
                    </a>
                </div>
            </div>
        </div>
        <div class="absolute top-0 left-1/2 -translate-x-1/2 w-full max-w-7xl h-full pointer-events-none opacity-30 dark:opacity-10">
            <div class="absolute top-12 left-10 w-72 h-72 bg-brand-500 rounded-full blur-3xl"></div>
            <div class="absolute bottom-12 right-10 w-96 h-96 bg-emerald-500 rounded-full blur-3xl"></div>
        </div>
    </section>

    <hr class="border-gray-200 dark:border-gray-800 max-w-7xl mx-auto">

    <section id="recursos" class="py-20 max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center max-w-3xl mx-auto mb-16">
            <h2 class="text-3xl font-bold text-gray-900 dark:text-white sm:text-4xl">Arquitetura de Alta Performance</h2>
            <p class="mt-4 text-gray-600 dark:text-gray-400">Funcionalidades nativas modernas focadas na experiência do usuário.</p>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <div class="bg-white dark:bg-gray-900 p-8 rounded-2xl border border-gray-200 dark:border-gray-800 shadow-sm hover:shadow-md transition">
                <div class="w-12 h-12 rounded-xl bg-brand-50 dark:bg-brand-900/20 flex items-center justify-center text-brand-600 dark:text-brand-500 mb-6">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path></svg>
                </div>
                <h3 class="text-xl font-semibold mb-2">Desempenho Extremo</h3>
                <p class="text-gray-600 dark:text-gray-400 text-sm">Carregamento quase instantâneo estruturado com semântica HTML5 limpa e otimizada.</p>
            </div>

            <div class="bg-white dark:bg-gray-900 p-8 rounded-2xl border border-gray-200 dark:border-gray-800 shadow-sm hover:shadow-md transition">
                <div class="w-12 h-12 rounded-xl bg-brand-50 dark:bg-brand-900/20 flex items-center justify-center text-brand-600 dark:text-brand-500 mb-6">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M20.354 15.354A9 9 0 018.646 3.646 9.003 9.003 0 0012 21a9.003 9.003 0 008.354-5.646z"></path></svg>
                </div>
                <h3 class="text-xl font-semibold mb-2">Modo Escuro Nativo</h3>
                <p class="text-gray-600 dark:text-gray-400 text-sm">Detecta automaticamente a preferência do sistema operacional e salva a escolha do usuário.</p>
            </div>

            <div class="bg-white dark:bg-gray-900 p-8 rounded-2xl border border-gray-200 dark:border-gray-800 shadow-sm hover:shadow-md transition">
                <div class="w-12 h-12 rounded-xl bg-brand-50 dark:bg-brand-900/20 flex items-center justify-center text-brand-600 dark:text-brand-500 mb-6">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 5a1 1 0 011-1h14a1 1 0 011 1v2a1 1 0 01-1 1H5a1 1 0 01-1-1V5zM4 13a1 1 0 011-1h6a1 1 0 011 1v6a1 1 0 01-1 1H5a1 1 0 01-1-1v-6zM16 13a1 1 0 011-1h2a1 1 0 011 1v6a1 1 0 01-1 1h-2a1 1 0 01-1-1v-6z"></path></svg>
                </div>
                <h3 class="text-xl font-semibold mb-2">Responsivo & Fluído</h3>
                <p class="text-gray-600 dark:text-gray-400 text-sm">Adaptável a qualquer tamanho de tela, desde smartphones antigos até monitores ultrawide.</p>
            </div>
        </div>
    </section>

    <footer class="bg-gray-100 dark:bg-gray-900 mt-20 border-t border-gray-200 dark:border-gray-800 transition-colors">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8 flex flex-col sm:flex-row items-center justify-between gap-4 text-sm text-gray-500">
            <p>&copy; 2026 Seu Nome / Projeto. Licença MIT.</p>
            <div class="flex gap-6">
                <a href="#" class="hover:text-gray-900 dark:hover:text-white transition">Privacidade</a>
                <a href="#" class="hover:text-gray-900 dark:hover:text-white transition">Termos</a>
            </div>
        </div>
    </footer>

    <script>
        const themeToggleDarkIcon = document.getElementById('theme-toggle-dark-icon');
        const themeToggleLightIcon = document.getElementById('theme-toggle-light-icon');
        const themeToggleBtn = document.getElementById('theme-toggle');

        // Define os ícones com base na escolha atual
        if (localStorage.getItem('color-theme') === 'dark' || (!('color-theme' in localStorage) && window.matchMedia('(prefers-color-scheme: dark)').matches)) {
            themeToggleLightIcon.classList.remove('hidden');
            document.documentElement.classList.add('dark');
        } else {
            themeToggleDarkIcon.classList.remove('hidden');
            document.documentElement.classList.remove('dark');
        }

        // Evento de clique para mudar o tema
        themeToggleBtn.addEventListener('click', function() {
            themeToggleDarkIcon.classList.toggle('hidden');
            themeToggleLightIcon.classList.toggle('hidden');

            if (localStorage.getItem('color-theme')) {
                if (localStorage.getItem('color-theme') === 'light') {
                    document.documentElement.classList.add('dark');
                    localStorage.setItem('color-theme', 'dark');
                } else {
                    document.documentElement.classList.remove('dark');
                    localStorage.setItem('color-theme', 'light');
                }
            } else {
                if (document.documentElement.classList.contains('dark')) {
                    document.documentElement.classList.remove('dark');
                    localStorage.setItem('color-theme', 'light');
                } else {
                    document.documentElement.classList.add('dark');
                    localStorage.setItem('color-theme', 'dark');
                }
            }
        });
    </script>
</body>
</html>
