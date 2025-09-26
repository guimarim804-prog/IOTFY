<!DOCTYPE html>  
<html lang="pt-BR">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>IOTFY - Automação Inteligente</title>  
    <script src="https://cdn.tailwindcss.com"></script>  
    <style>  
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');  
        body { font-family: 'Inter', sans-serif; }  
          
        .gradient-bg {  
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);  
        }  
          
        .card-hover {  
            transition: transform 0.3s ease, box-shadow 0.3s ease;  
        }  
          
        .card-hover:hover {  
            transform: translateY(-5px);  
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);  
        }  
          
        .pulse-animation {  
            animation: pulse 2s infinite;  
        }  
          
        @keyframes pulse {  
            0%, 100% { opacity: 1; }  
            50% { opacity: 0.7; }  
        }  
          
        .fade-in {  
            animation: fadeIn 1s ease-in;  
        }  
          
        @keyframes fadeIn {  
            from { opacity: 0; transform: translateY(30px); }  
            to { opacity: 1; transform: translateY(0); }  
        }  
    </style>  
</head>  
<body class="bg-gray-50">  
    <!-- Header -->  
    <header class="gradient-bg text-white shadow-lg">  
        <nav class="container mx-auto px-6 py-4">  
            <div class="flex items-center justify-between">  
                <div class="flex items-center space-x-2">  
                    <div class="w-10 h-10 bg-white rounded-lg flex items-center justify-center">  
                        <span class="text-2xl">🏠</span>  
                    </div>  
                    <h1 class="text-2xl font-bold">IOTFY</h1>  
                </div>  
                <div class="hidden md:flex space-x-6">  
                    <a href="#produto" class="hover:text-blue-200 transition-colors">Produto</a>  
                    <a href="#recursos" class="hover:text-blue-200 transition-colors">Recursos</a>  
                    <a href="#contatos" class="hover:text-blue-200 transition-colors">Contatos</a>  
                </div>  
            </div>  
        </nav>  
    </header>  
  
    <!-- Hero Section -->  
    <section class="gradient-bg text-white py-20">  
        <div class="container mx-auto px-6 text-center">  
            <div class="fade-in">  
                <h2 class="text-5xl md:text-6xl font-bold mb-6">  
                    O Futuro da <span class="text-yellow-300">Automação</span> Residencial e Industrial  
                </h2>  
                <p class="text-xl md:text-2xl mb-8 max-w-3xl mx-auto opacity-90">  
                    Controle sua casa/empresas inteira com um toque. IOTFY conecta todos os seus dispositivos em um sistema inteligente e intuitivo.  
                </p>  
                <button onclick="scrollToSection('produto')" class="bg-white text-purple-600 px-8 py-4 rounded-full text-lg font-semibold hover:bg-gray-100 transition-colors shadow-lg">  
                    Descobrir Mais  
                </button>  
            </div>  
        </div>  
    </section>  
  
    <!-- Produto Section -->  
    <section id="produto" class="py-20 bg-white">  
        <div class="container mx-auto px-6">  
            <div class="text-center mb-16">  
                <h3 class="text-4xl font-bold text-gray-800 mb-4">IOTFY</h3>  
                <p class="text-xl text-gray-600 max-w-2xl mx-auto">  
                    O centro de controle inteligente que revoluciona a forma como você interage com sua casa  
                </p>  
            </div>  
              
            <div class="grid md:grid-cols-2 gap-12 items-center">  
                <div class="space-y-6">  
                    <div class="bg-gradient-to-r from-blue-500 to-purple-600 p-8 rounded-2xl text-white">  
                        <div class="w-16 h-16 bg-white rounded-full flex items-center justify-center mb-4">  
                            <span class="text-3xl">🎛️</span>  
                        </div>  
                        <h4 class="text-2xl font-bold mb-3">Controle Centralizado</h4>  
                        <p class="text-lg opacity-90">  
                            Um único dispositivo para controlar luzes, temperatura, segurança, eletrodomésticos e muito mais.  
                        </p>  
                    </div>  
                      
                    <div class="grid grid-cols-2 gap-4">  
                        <div class="bg-gray-50 p-6 rounded-xl text-center">  
                            <span class="text-3xl mb-2 block">📱</span>  
                            <h5 class="font-semibold text-gray-800">App Móvel</h5>  
                            <p class="text-sm text-gray-600">Controle remoto total</p>  
                        </div>  
                        <div class="bg-gray-50 p-6 rounded-xl text-center">  
                            <span class="text-3xl mb-2 block">🗣️</span>  
                            <h5 class="font-semibold text-gray-800">Comando de Voz</h5>  
                            <p class="text-sm text-gray-600">Sua casa a sua disposição</p>  
                        </div>  
                    </div>  
                </div>  
                  
                <div class="relative">  
                    <div class="bg-gradient-to-br from-gray-100 to-gray-200 rounded-3xl p-8 shadow-2xl">  
                        <div class="bg-white rounded-2xl p-6 mb-6 shadow-lg">  
                            <div class="flex items-center justify-between mb-4">  
                                <h5 class="font-bold text-gray-800">Status da Casa</h5>  
                                <div class="w-3 h-3 bg-green-500 rounded-full pulse-animation"></div>  
                            </div>  
                            <div class="space-y-3">  
                                <div class="flex justify-between items-center">  
                                    <span class="text-gray-600">🌡️ Temperatura</span>  
                                    <span class="font-semibold">22°C</span>  
                                </div>  
                                <div class="flex justify-between items-center">  
                                    <span class="text-gray-600">💡 Luzes Ativas</span>  
                                    <span class="font-semibold">5/12</span>  
                                </div>  
                                <div class="flex justify-between items-center">  
                                    <span class="text-gray-600">🔒 Segurança</span>  
                                    <span class="font-semibold text-green-600">Ativa</span>  
                                </div>  
                            </div>  
                        </div>  
                          
                        <div class="grid grid-cols-2 gap-4">  
                            <button class="bg-blue-500 text-white p-4 rounded-xl font-semibold hover:bg-blue-600 transition-colors">  
                                🏠 Modo Casa  
                            </button>  
                            <button class="bg-purple-500 text-white p-4 rounded-xl font-semibold hover:bg-purple-600 transition-colors">  
                                🌙 Modo Noite  
                            </button>  
                        </div>  
                    </div>  
                </div>  
            </div>  
        </div>  
    </section>  
  
    <!-- Recursos Section -->  
    <section id="recursos" class="py-20 bg-gray-50">  
        <div class="container mx-auto px-6">  
            <div class="text-center mb-16">  
                <h3 class="text-4xl font-bold text-gray-800 mb-4">Recursos Principais</h3>  
                <p class="text-xl text-gray-600">Tecnologia avançada para uma vida mais inteligente</p>  
            </div>  
              
            <div class="grid md:grid-cols-3 gap-8">  
                <div class="bg-white p-8 rounded-2xl shadow-lg card-hover">  
                    <div class="w-16 h-16 bg-blue-100 rounded-full flex items-center justify-center mb-6">  
                        <span class="text-3xl">🤖</span>  
                    </div>  
                    <h4 class="text-xl font-bold text-gray-800 mb-4">MQTT Integrado</h4>  
                    <p class="text-gray-600">  
                       1. Broker  
É o servidor central que gerencia todas as mensagens.  
2. Cliente  
Pode ser um dispositivo (ESP32).  
Envia e recebe mensagens.  
3. Tópico  
É como o "assunto" da mensagem.  
Ex: casa/luz/sala ou sensor/temperatura.  
4. Publicar (Publish)  
O cliente envia uma mensagem para um tópico.  
5. Assinar (Subscribe)  
O cliente se inscreve em um tópico para receber mensagem  
                    </p>  
                </div>  
                  
                <div class="bg-white p-8 rounded-2xl shadow-lg card-hover">  
                    <div class="w-16 h-16 bg-green-100 rounded-full flex items-center justify-center mb-6">  
                        <span class="text-3xl">⌨️</span>  
                    </div>  
                    <h4 class="text-xl font-bold text-gray-800 mb-4">ESP REINMAKER</h4>  
                    <p class="text-gray-600">  
                       Escolhemos a ESP RainMaker porque ela conecta-se à nuvem, permitindo controlar a automação de qualquer lugar, sem depender da mesma rede Wi-Fi, como acontece com o MQTT.  
Além disso, ela gera seu próprio aplicativo, dispensando a criação de apps, e oferece uma interface prática e personalizada.  
                    </p>  
                </div>  
                  
                <div class="bg-white p-8 rounded-2xl shadow-lg card-hover">  
                    <div class="w-16 h-16 bg-purple-100 rounded-full flex items-center justify-center mb-6">  
                        <span class="text-3xl">⚡</span>  
                    </div>  
                    <h4 class="text-xl font-bold text-gray-800 mb-4">IOTFY ONE</h4>  
                    <p class="text-gray-600">  
                        A placa IOTFY ONE é voltada para monitoramento e atuação com base em dados de sensores, coletando informações de variáveis ambientais, elétricas e outras.  
Ela é usada em diversas aplicações, como o controle e acompanhamento de variáveis elétricas e ambientais em diferentes contextos.  
                    </p>  
                </div>  
            </div>  
        </div>  
    </section>  
  
    <!-- Contatos Section -->  
    <section id="contatos" class="py-20 bg-white">  
        <div class="container mx-auto px-6">  
            <div class="text-center mb-16">  
                <h3 class="text-4xl font-bold text-gray-800 mb-4">Entre em Contato</h3>  
                <p class="text-xl text-gray-600">Estamos aqui para ajudar você a transformar sua casa</p>  
            </div>  
              
            <div class="max-w-4xl mx-auto">  
                <div class="grid md:grid-cols-2 gap-8">  
                    <!-- Contatos Diretos -->  
                    <div class="space-y-6">  
                        <h4 class="text-2xl font-bold text-gray-800 mb-6">Fale Conosco</h4>  
                          
                        <a href="https://wa.me/5511913305213" target="_blank" rel="noopener noreferrer"   
                           class="flex items-center space-x-4 p-4 bg-green-50 rounded-xl hover:bg-green-100 transition-colors card-hover">  
                            <div class="w-12 h-12 bg-green-500 rounded-full flex items-center justify-center">  
                                <svg class="w-6 h-6 text-white" fill="currentColor" viewBox="0 0 24 24">  
                                    <path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893A11.821 11.821 0 0020.885 3.488"/>  
                                </svg>  
                            </div>  
                            <div>  
                                <h5 class="font-semibold text-gray-800">WhatsApp</h5>  
                                <p class="text-gray-600">(11) 91330-5213</p>  
                            </div>  
                        </a>  
                          
                        <a href="mailto:empresa.iotfy@gmail.com" target="_blank" rel="noopener noreferrer"  
                           class="flex items-center space-x-4 p-4 bg-red-50 rounded-xl hover:bg-red-100 transition-colors card-hover">  
                            <div class="w-12 h-12 bg-red-500 rounded-full flex items-center justify-center">  
                                <svg class="w-6 h-6 text-white" fill="currentColor" viewBox="0 0 24 24">  
                                    <path d="M24 5.457v13.909c0 .904-.732 1.636-1.636 1.636h-3.819V11.73L12 16.64l-6.545-4.91v9.273H1.636A1.636 1.636 0 0 1 0 19.366V5.457c0-.904.732-1.636 1.636-1.636h.749L12 10.724l9.615-6.903h.749c.904 0 1.636.732 1.636 1.636z"/>  
                                </svg>  
                            </div>  
                            <div>  
                                <h5 class="font-semibold text-gray-800">Gmail</h5>  
                                <p class="text-gray-600">empresa.iotfy@gmail.com</p>  
                            </div>  
                        </a>  
                          
                        <a href="https://instagram.com/iot.fy" target="_blank" rel="noopener noreferrer"  
                           class="flex items-center space-x-4 p-4 bg-pink-50 rounded-xl hover:bg-pink-100 transition-colors card-hover">  
                            <div class="w-12 h-12 bg-pink-500 rounded-full flex items-center justify-center">  
                                <svg class="w-6 h-6 text-white" fill="currentColor" viewBox="0 0 24 24">  
                                    <path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.25gmail.com2.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"/>  
                                </svg>  
                            </div>  
                            <div>  
                                <h5 class="font-semibold text-gray-800">Instagram</h5>  
                                <p class="text-gray-600">@IOT.FY</p>  
                            </div>  
                        </a>  
                          
                        <a href="https://t.me/iotfybr" target="_blank" rel="noopener noreferrer"  
                           class="flex items-center space-x-4 p-4 bg-blue-50 rounded-xl hover:bg-blue-100 transition-colors card-hover">  
                            <div class="w-12 h-12 bg-blue-500 rounded-full flex items-center justify-center">  
                                <svg class="w-6 h-6 text-white" fill="currentColor" viewBox="0 0 24 24">  
                                    <path d="M11.944 0A12 12 0 0 0 0 12a12 12 0 0 0 12 12 12 12 0 0 0 12-12A12 12 0 0 0 12 0a12 12 0 0 0-.056 0zm4.962 7.224c.1-.002.321.023.465.14a.506.506 0 0 1 .171.325c.016.093.036.306.02.472-.18 1.898-.962 6.502-1.36 8.627-.168.9-.499 1.201-.82 1.23-.696.065-1.225-.46-1.9-.902-1.056-.693-1.653-1.124-2.678-1.8-1.185-.78-.417-1.21.258-1.91.177-.184 3.247-2.977 3.307-3.23.007-.032.014-.15-.056-.212s-.174-.041-.249-.024c-.106.024-1.793 1.14-5.061 3.345-.48.33-.913.49-1.302.48-.428-.008-1.252-.241-1.865-.44-.752-.245-1.349-.374-1.297-.789.027-.216.325-.437.893-.663 3.498-1.524 5.83-2.529 6.998-3.014 3.332-1.386 4.025-1.627 4.476-1.635z"/>  
                                </svg>  
                            </div>  
                            <div>  
                                <h5 class="font-semibold text-gray-800">Telegram</h5>  
                                <p class="text-gray-600">@IOTFYBR</p>  
                            </div>  
                        </a>  
                    </div>  
                      
                    <!-- Formulário de Contato -->  
                    <div class="bg-gray-50 p-8 rounded-2xl">  
                        <h4 class="text-2xl font-bold text-gray-800 mb-6">Envie uma Mensagem</h4>  
                        <form onsubmit="handleFormSubmit(event)" class="space-y-4">  
                            <div>  
                                <label class="block text-gray-700 font-medium mb-2">Nome</label>  
                                <input type="text" required class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-purple-500 focus:border-transparent">  
                            </div>  
                            <div>  
                                <label class="block text-gray-700 font-medium mb-2">Email</label>  
                                <input type="email" required class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-purple-500 focus:border-transparent">  
                            </div>  
                            <div>  
                                <label class="block text-gray-700 font-medium mb-2">Mensagem</label>  
                                <textarea rows="4" required class="w-full p-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-purple-500 focus:border-transparent"></textarea>  
                            </div>  
                            <button type="submit" class="w-full bg-purple-600 text-white py-3 rounded-lg font-semibold hover:bg-purple-700 transition-colors">  
                                Enviar Mensagem  
                            </button>  
                        </form>  
                        <div id="form-message" class="mt-4 p-3 rounded-lg hidden"></div>  
                    </div>  
                </div>  
            </div>  
        </div>  
    </section>  
  
    <!-- Footer -->  
    <footer class="bg-gray-800 text-white py-12">  
        <div class="container mx-auto px-6">  
            <div class="text-center">  
                <div class="flex items-center justify-center space-x-2 mb-4">  
                    <div class="w-10 h-10 bg-purple-600 rounded-lg flex items-center justify-center">  
                        <span class="text-2xl">🏠</span>  
                    </div>  
                    <h3 class="text-2xl font-bold">IOTFY</h3>  
                </div>  
                <p class="text-gray-400 mb-6">Transformando casas em lares inteligentes</p>  
                <p class="text-gray-500">&copy; 2024 IOTFY. Todos os direitos reservados.</p>  
            </div>  
        </div>  
    </footer>  
  
    <script>  
        function scrollToSection(sectionId) {  
            document.getElementById(sectionId).scrollIntoView({  
                behavior: 'smooth'  
            });  
        }  
  
        function handleFormSubmit(event) {  
            event.preventDefault();  
              
            const messageDiv = document.getElementById('form-message');  
            messageDiv.className = 'mt-4 p-3 rounded-lg bg-green-100 text-green-800';  
            messageDiv.textContent = 'Mensagem enviada com sucesso! Entraremos em contato em breve.';  
            messageDiv.classList.remove('hidden');  
              
            // Reset form  
            event.target.reset();  
              
            // Hide message after 5 seconds  
            setTimeout(() => {  
                messageDiv.classList.add('hidden');  
            }, 5000);  
        }  
  
        // Smooth scroll for navigation links  
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {  
            anchor.addEventListener('click', function (e) {  
                e.preventDefault();  
                const target = document.querySelector(this.getAttribute('href'));  
                if (target) {  
                    target.scrollIntoView({  
                        behavior: 'smooth'  
                    });  
                }  
            });  
        });  
    </script>  
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'9832bfe066a51a9a',t:'MTc1ODU1NDA0MC4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>  
</html>  
  
  
- [ ]   
