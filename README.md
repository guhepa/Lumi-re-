<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lumière Campus - Arte Acessível para Todos</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Raleway:wght@300;400;600&display=swap');
        
        body {
            font-family: 'Raleway', sans-serif;
            scroll-behavior: smooth;
        }
        
        .title-font {
            font-family: 'Playfair Display', serif;
        }
        
        .hero-pattern {
            background-color: #fef9e7;
            background-image: url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%23f9e79f' fill-opacity='0.4'%3E%3Cpath d='M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
        }
        
        .course-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1);
        }
        
        .transition-all {
            transition: all 0.3s ease;
        }
        
        .floating {
            animation: floating 3s ease-in-out infinite;
        }
        
        @keyframes floating {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-15px); }
            100% { transform: translateY(0px); }
        }
        
        .mobile-menu {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease-out;
        }
        
        .mobile-menu.open {
            max-height: 500px;
        }
    </style>
</head>
<body class="bg-amber-50">
    <!-- Header/Navigation -->
    <header class="sticky top-0 z-50 bg-amber-100 shadow-md">
        <div class="container mx-auto px-4 py-3 flex justify-between items-center">
            <div class="flex items-center">
                <i class="fas fa-palette text-amber-600 text-2xl mr-2"></i>
                <h1 class="title-font text-2xl font-bold text-amber-800">LUMIÈRE CAMPUS</h1>
            </div>
            <nav class="hidden md:block">
                <ul class="flex space-x-8">
                    <li><a href="#inicio" class="text-amber-700 hover:text-amber-900 font-medium transition-all">Início</a></li>
                    <li><a href="#cursos" class="text-amber-700 hover:text-amber-900 font-medium transition-all">Cursos</a></li>
                    <li><a href="#vestibular" class="text-amber-700 hover:text-amber-900 font-medium transition-all">Vestibular</a></li>
                    <li><a href="#sobre" class="text-amber-700 hover:text-amber-900 font-medium transition-all">Sobre Nós</a></li>
                    <li><a href="#contato" class="text-amber-700 hover:text-amber-900 font-medium transition-all">Contato</a></li>
                </ul>
            </nav>
            <button id="mobile-menu-button" class="md:hidden text-amber-700 focus:outline-none">
                <i class="fas fa-bars text-2xl"></i>
            </button>
        </div>
        
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="mobile-menu md:hidden bg-amber-50">
            <div class="container mx-auto px-4 py-3">
                <ul class="space-y-3">
                    <li><a href="#inicio" class="block text-amber-700 hover:text-amber-900 font-medium py-2 transition-all">Início</a></li>
                    <li><a href="#cursos" class="block text-amber-700 hover:text-amber-900 font-medium py-2 transition-all">Cursos</a></li>
                    <li><a href="#vestibular" class="block text-amber-700 hover:text-amber-900 font-medium py-2 transition-all">Vestibular</a></li>
                    <li><a href="#sobre" class="block text-amber-700 hover:text-amber-900 font-medium py-2 transition-all">Sobre Nós</a></li>
                    <li><a href="#contato" class="block text-amber-700 hover:text-amber-900 font-medium py-2 transition-all">Contato</a></li>
                </ul>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="inicio" class="hero-pattern py-20">
        <div class="container mx-auto px-4 flex flex-col md:flex-row items-center">
            <div class="md:w-1/2 mb-10 md:mb-0">
                <h2 class="title-font text-4xl md:text-5xl font-bold text-amber-800 mb-6">Arte Acessível para Todos</h2>
                <p class="text-amber-700 text-lg mb-8">No Lumière Campus, acreditamos que a arte é um direito de todos. Oferecemos cursos de qualidade a preços acessíveis e bolsas integrais através do nosso vestibular social.</p>
                <div class="flex flex-col sm:flex-row space-y-4 sm:space-y-0 sm:space-x-4">
                    <a href="#cursos" class="bg-amber-500 hover:bg-amber-600 text-white font-bold py-3 px-6 rounded-lg shadow-md transition-all text-center">Nossos Cursos</a>
                    <a href="#vestibular" class="bg-amber-100 hover:bg-amber-200 text-amber-800 font-bold py-3 px-6 rounded-lg shadow-md transition-all text-center">Vestibular Social</a>
                </div>
            </div>
            <div class="md:w-1/2 flex justify-center">
                <div class="relative w-full max-w-md">
                    <div class="absolute -top-6 -left-6 w-32 h-32 bg-amber-200 rounded-full opacity-70"></div>
                    <div class="absolute -bottom-6 -right-6 w-32 h-32 bg-amber-300 rounded-full opacity-70"></div>
                    <img src="https://images.unsplash.com/photo-1547153760-18fc86324498?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=687&q=80" alt="Estudantes de arte" class="relative z-10 rounded-lg shadow-xl w-full h-auto floating">
                </div>
            </div>
        </div>
    </section>

    <!-- Courses Section -->
    <section id="cursos" class="py-16 bg-amber-50">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16">
                <h2 class="title-font text-3xl md:text-4xl font-bold text-amber-800 mb-4">Nossos Cursos</h2>
                <p class="text-amber-700 max-w-2xl mx-auto">Oferecemos uma variedade de cursos artísticos com mensalidades acessíveis (R$80-R$120) e bolsas integrais através do vestibular social.</p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Dança -->
                <div class="course-card bg-white rounded-xl shadow-md overflow-hidden transition-all">
                    <div class="h-48 bg-amber-200 flex items-center justify-center">
                        <i class="fas fa-child-reaching text-6xl text-amber-700"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="title-font text-xl font-bold text-amber-800 mb-2">Dança</h3>
                        <ul class="text-amber-700 space-y-2">
                            <li class="flex items-center"><i class="fas fa-check-circle text-amber-500 mr-2"></i> Ballet Clássico</li>
                            <li class="flex items-center"><i class="fas fa-check-circle text-amber-500 mr-2"></i> Dança Contemporânea</li>
                            <li class="flex items-center"><i class="fas fa-check-circle text-amber-500 mr-2"></i> Jazz Dance</li>
                            <li class="flex items-center"><i class="fas fa-check-circle text-amber-500 mr-2"></i> Danças Urbanas</li>
                        </ul>
                        <div class="mt-4">
                            <span class="inline-block bg-amber-100 text-amber-800 px-3 py-1 rounded-full text-sm font-semibold">R$100/mês</span>
                        </div>
                    </div>
                </div>
                
                <!-- Música -->
                <div class="course-card bg-white rounded-xl shadow-md overflow-hidden transition-all">
                    <div class="h-48 bg-amber-300 flex items-center justify-center">
                        <i class="fas fa-music text-6xl text-amber-800"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="title-font text-xl font-bold text-amber-800 mb-2">Música</h3>
                        <ul class="text-amber-700 space-y-2">
                            <li class="flex items-center"><i class="fas fa-check-circle text-amber-500 mr-2"></i> Piano</li>
                            <li class="flex items-center"><i class="fas fa-check-circle text-amber-500 mr-2"></i> Teclado</li>
                            <li class="flex items-center"><i class="fas fa-check-circle text-amber-500 mr-2"></i> Composição Musical</li>
                            <li class="flex items-center"><i class="fas fa-check-circle text-amber-500 mr-2"></i> Canto</li>
                            <li class="flex items-center"><i class="fas fa-check-circle text-amber-500 mr-2"></i> Violão</li>
                        </ul>
                        <div class="mt-4">
                            <span class="inline-block bg-amber-100 text-amber-800 px-3 py-1 rounded-full text-sm font-semibold">R$120/mês</span>
                        </div>
                    </div>
                </div>
                
                <!-- Artes Visuais -->
                <div class="course-card bg-white rounded-xl shadow-md overflow-hidden transition-all">
                    <div class="h-48 bg-amber-400 flex items-center justify-center">
                        <i class="fas fa-paintbrush text-6xl text-amber-900"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="title-font text-xl font-bold text-amber-800 mb-2">Artes Visuais</h3>
                        <ul class="text-amber-700 space-y-2">
                            <li class="flex items-center"><i class="fas fa-check-circle text-amber-500 mr-2"></i> Desenho Artístico</li>
                            <li class="flex items-center"><i class="fas fa-check-circle text-amber-500 mr-2"></i> Pintura</li>
                            <li class="flex items-center"><i class="fas fa-check-circle text-amber-500 mr-2"></i> Fotografia</li>
                            <li class="flex items-center"><i class="fas fa-check-circle text-amber-500 mr-2"></i> Escultura</li>
                        </ul>
                        <div class="mt-4">
                            <span class="inline-block bg-amber-100 text-amber-800 px-3 py-1 rounded-full text-sm font-semibold">R$90/mês</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Vestibular Social Section -->
    <section id="vestibular" class="py-16 bg-amber-100">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 mb-10 md:mb-0 md:pr-10">
                    <h2 class="title-font text-3xl md:text-4xl font-bold text-amber-800 mb-6">Vestibular Social</h2>
                    <p class="text-amber-700 mb-6">Nosso vestibular social oferece bolsas de estudo integrais para estudantes talentosos que não têm condições financeiras para arcar com os custos dos cursos.</p>
                    <p class="text-amber-700 mb-6">O processo seletivo avalia o talento artístico e a situação socioeconômica do candidato, sem qualquer custo de inscrição.</p>
                    <div class="bg-amber-50 p-6 rounded-lg shadow-inner">
                        <h3 class="title-font text-xl font-bold text-amber-800 mb-3">Próximas Datas</h3>
                        <ul class="space-y-3">
                            <li class="flex items-start">
                                <i class="fas fa-calendar-check text-amber-500 mt-1 mr-3"></i>
                                <div>
                                    <p class="font-semibold text-amber-800">Inscrições:</p>
                                    <p class="text-amber-700">01/08 a 30/08</p>
                                </div>
                            </li>
                            <li class="flex items-start">
                                <i class="fas fa-pencil-alt text-amber-500 mt-1 mr-3"></i>
                                <div>
                                    <p class="font-semibold text-amber-800">Provas Práticas:</p>
                                    <p class="text-amber-700">10/09</p>
                                </div>
                            </li>
                            <li class="flex items-start">
                                <i class="fas fa-award text-amber-500 mt-1 mr-3"></i>
                                <div>
                                    <p class="font-semibold text-amber-800">Resultado:</p>
                                    <p class="text-amber-700">25/09</p>
                                </div>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="md:w-1/2">
                    <div class="bg-white p-8 rounded-xl shadow-lg">
                        <h3 class="title-font text-2xl font-bold text-amber-800 mb-6 text-center">Fique Atualizado</h3>
                        <p class="text-amber-700 mb-6 text-center">Cadastre-se para receber informações sobre o próximo vestibular social e nossas atividades.</p>
                        <form class="space-y-4">
                            <div>
                                <label for="name" class="block text-amber-700 font-medium mb-1">Nome Completo</label>
                                <input type="text" id="name" class="w-full px-4 py-2 border border-amber-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-amber-500">
                            </div>
                            <div>
                                <label for="email" class="block text-amber-700 font-medium mb-1">E-mail</label>
                                <input type="email" id="email" class="w-full px-4 py-2 border border-amber-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-amber-500">
                            </div>
                            <div>
                                <label for="interest" class="block text-amber-700 font-medium mb-1">Área de Interesse</label>
                                <select id="interest" class="w-full px-4 py-2 border border-amber-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-amber-500">
                                    <option value="">Selecione...</option>
                                    <option value="danca">Dança</option>
                                    <option value="musica">Música</option>
                                    <option value="artes-visuais">Artes Visuais</option>
                                </select>
                            </div>
                            <button type="submit" class="w-full bg-amber-500 hover:bg-amber-600 text-white font-bold py-3 px-4 rounded-lg shadow-md transition-all">Cadastrar</button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="sobre" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16">
                <h2 class="title-font text-3xl md:text-4xl font-bold text-amber-800 mb-4">Sobre o Lumière Campus</h2>
                <p class="text-amber-700 max-w-3xl mx-auto">Um projeto social que nasceu da crença de que a arte transforma vidas e deve ser acessada por todos, independentemente de sua condição financeira.</p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div class="bg-amber-50 p-6
</html>
