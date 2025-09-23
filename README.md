
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>La Barra Marina</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://lh3.googleusercontent.com/p/AF1QipPJqix-vFSUjv_8d50UXOq2nFAI6OZ8d6sn3RVw=s680-w680-h510-rw?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/qrcodejs@1.0.0/qrcode.min.js"></script>
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f7f9fc;
        }
        .bg-cover-image {
            background-image: url('https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgetWtWiFafJ6S44D1d2hfyV5U3AUQpLaQMUZEANV7oJPMGl4XeGTOIOOAIJLZCyC431-CFN5q43qRe7OibKgPTSlBZhGUq_4jjm7zbK8Oi28ioPWxfyhYJzQAXdq4frIhgTR1C30riiqh2/s752/Sin+t%25C3%25ADtulo-2.jpg');
            background-position: center;
            background-size: cover;
        }
    </style>
</head>
<body class="bg-gray-100 text-gray-800">

    <!-- Chosen Palette: Coastal Blue and Warm Sand -->
    <!-- Application Structure Plan: The application uses a single-page structure with vertical scrolling, starting with a captivating hero image, followed by an "About Us" section, the complete interactive menu, and a footer with contact details and QR codes. This structure is intuitive for users and guides them naturally from the brand's identity to the core offering (the menu). The menu itself is organized thematically (Seafood, Meats, Kids, Drinks) rather than by the original file structure, which allows customers to find what they are looking for more easily. Interactive elements like Text-to-Speech and dynamic pairings are included to increase engagement and accessibility. -->
    <!-- Visualization & Content Choices: The menu information is primarily textual and is best organized into distinct categories. Goal: Inform & Organize. Presentation Method: A responsive card-based grid layout using HTML and Tailwind CSS. Each card represents a dish or a group of related dishes (e.g., all trout preparations under one card) to keep the layout clean and scannable. Interaction: Subtle hover animations on cards provide visual feedback. Buttons trigger JavaScript functions for Text-to-Speech (accessibility) and pairing suggestions (engagement). A search bar with a JavaScript filter is added to improve navigation and user experience. Justification: This card grid is a highly effective and standard UX pattern for digital menus, as it allows users to easily compare options. No charts are necessary as the data is qualitative. No SVG/Mermaid is used, relying on CSS and placeholder images for visuals. -->
    <!-- CONFIRMATION: NO SVG graphics used. NO Mermaid JS used. -->

    <!-- Header & Hero Section -->
    <header class="bg-cover-image h-screen relative flex items-center justify-center text-white">
        <div class="absolute inset-0 bg-black opacity-50"></div>
        <div class="container mx-auto px-4 text-center relative z-10">
            <h1 class="text-5xl md:text-7xl font-bold mb-4">La Barra Marina</h1>
            <p class="text-xl md:text-2xl font-semibold mb-8">El mejor sabor del mar en Melgar</p>
            <a href="#menu" class="bg-blue-600 hover:bg-blue-700 text-white font-bold py-3 px-8 rounded-full shadow-lg transition duration-300 transform hover:scale-105">
                Ver Menú
            </a>
        </div>
    </header>

    <!-- About Us Section -->
    <section id="nosotros" class="py-16 md:py-24 bg-white">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row items-center gap-8">
                <div class="md:w-1/2">
                    <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgetWtWiFafJ6S44D1d2hfyV5U3AUQpLaQMUZEANV7oJPMGl4XeGTOIOOAIJLZCyC431-CFN5q43qRe7OibKgPTSlBZhGUq_4jjm7zbK8Oi28ioPWxfyhYJzQAXdq4frIhgTR1C30riiqh2/s752/Sin+t%25C3%25ADtulo-2.jpg" alt="Interior del restaurante La Barra Marina" class="rounded-lg shadow-xl w-full h-auto object-cover">
                </div>
                <div class="md:w-1/2 text-center md:text-left">
                    <h2 class="text-4xl font-bold text-gray-900 mb-4">Nuestra Historia</h2>
                    <p class="text-lg text-gray-700 leading-relaxed mb-4">
                        En La Barra Marina, nos dedicamos a traer los sabores más frescos y auténticos del mar a la hermosa ciudad de Melgar. Con años de experiencia y una pasión por la cocina, cada plato es preparado con ingredientes de la más alta calidad para ofrecerte una experiencia culinaria inolvidable.
                    </p>
                    <p class="text-lg text-gray-700 leading-relaxed">
                        Nuestro ambiente es relajado y familiar, perfecto para compartir momentos especiales con tus seres queridos. ¡Te esperamos para que descubras por qué somos el restaurante de mariscos favorito de la región!
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Menu Section -->
    <section id="menu" class="py-16 md:py-24 bg-gray-100">
        <div class="container mx-auto px-4">
            <h2 class="text-4xl font-bold text-center text-gray-900 mb-12">Nuestro Menú</h2>
            <div class="flex justify-center mb-8">
                <input type="text" id="searchInput" placeholder="Buscar en el menú..." class="p-3 rounded-full shadow-md w-full max-w-lg focus:outline-none focus:ring-2 focus:ring-blue-500 transition duration-300">
            </div>

            <!-- Chef's Recommendation Section (Static) -->
            <div class="bg-blue-500 rounded-lg shadow-lg p-6 mb-8 flex flex-col md:flex-row items-center text-white text-center md:text-left">
                <img src="https://lh3.googleusercontent.com/gps-cs-s/AC9h4np24xa27W1y4sVTL2TQP9cxbsJVBSJUYQ3-zSwNF3qEe2l3fGIrt04ezLoN2D8QlcYcVtAAFpteF5kCl37iVYu8KgqXPmN5KHcyr84Z3CubSvYUPcLLDiAaxuCOHzeNRW44hqKv=s680-w680-h510-rw?text=Cazuela+de+Mariscos" alt="Cazuela de Mariscos" class="rounded-lg mb-4 md:mb-0 md:mr-6 w-full md:w-auto h-auto object-cover">
                <div>
                    <h3 class="text-2xl font-bold mb-2">Recomendación del Chef ✨</h3>
                    <p class="text-lg">
                        ¡No te puedes perder la **Cazuela de Mariscos**! Una deliciosa y cremosa mezcla de camarones, calamar y pulpo, cocinados a fuego lento en una base natural de verduras y especias. Es el plato perfecto para calentar el alma.
                    </p>
                </div>
            </div>

            <!-- All Menu Items Container -->
            <div id="menuItemsContainer">
                
                <!-- New Appetizers (Entradas) Section -->
                <div class="mt-8 text-center">
                    <h2 class="text-4xl font-bold text-gray-900 mb-8">Entradas</h2>
                    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                        <!-- Canastas de Plátano -->
                        <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT5vYfkh6-mNbvyGSp0Kq5HCoGyUvj74QEI5w&s?text=Canastas+de+Platano" alt="Canastas de Plátano con Hogao" class="rounded-lg mb-4 w-full h-auto object-cover">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Canastas de Plátano con Hogao</h3>
                            <p class="text-gray-600 mb-4" data-description="Seis crujientes canastas de plátano macho, rellenas con nuestro tradicional hogao.">Seis crujientes canastas de plátano macho, rellenas con nuestro tradicional hogao.</p>
                            <span class="text-xl font-bold text-blue-600">12.000 pesos</span>
                            <div class="flex space-x-2 mt-4">
                                <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                                <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Canastas de Plátano">✨ Maridaje</button>
                            </div>
                            <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                        </div>
                        <!-- Copa de Ceviche -->
                        <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTJ2ldOvPgDKfLh9k8A3HqMrzGNw8UTkLrmeg&s?text=Copa+de+Ceviche" alt="Copa de Ceviche" class="rounded-lg mb-4 w-full h-auto object-cover">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Copa de Ceviche</h3>
                            <p class="text-gray-600 mb-4" data-description="Una porción perfecta de ceviche de mariscos frescos, servida en copa.">Una porción perfecta de ceviche de mariscos frescos, servida en copa.</p>
                            <span class="text-xl font-bold text-blue-600">$18.000 COP</span>
                            <div class="flex space-x-2 mt-4">
                                <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                                <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Copa de Ceviche">✨ Maridaje</button>
                            </div>
                            <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                        </div>
                    </div>
                </div>

                <!-- New Cazuelas Section -->
                <div class="mt-16 text-center">
                    <h2 class="text-4xl font-bold text-gray-900 mb-8">Cazuelas</h2>
                    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                        <!-- Cazuelas de Mariscos -->
                        <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                            <img src="https://lh3.googleusercontent.com/gps-cs-s/AC9h4np24xa27W1y4sVTL2TQP9cxbsJVBSJUYQ3-zSwNF3qEe2l3fGIrt04ezLoN2D8QlcYcVtAAFpteF5kCl37iVYu8KgqXPmN5KHcyr84Z3CubSvYUPcLLDiAaxuCOHzeNRW44hqKv=s680-w680-h510-rw?text=Cazuela+de+Mariscos" alt="Cazuela de Mariscos" class="rounded-lg mb-4 w-full h-auto object-cover">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Cazuelas de Mariscos</h3>
                            <div class="text-gray-600 text-left w-full">
                                <p class="mb-1" data-description="Cazuela de Mariscos.">Cazuela de Mariscos: <span class="text-blue-600 font-bold">$35.000 - $40.000</span></p>
                                <p class="mb-1" data-description="Cazuela Tsunami Marinera.">Cazuela Tsunami Marinera: <span class="text-blue-600 font-bold">$45.000</span></p>
                                <p class="mb-1" data-description="Cazuela de Mariscos con Langostinos.">Cazuela de Mariscos con Langostinos: <span class="text-blue-600 font-bold">$50.000</span></p>
                            </div>
                            <div class="flex space-x-2 mt-4">
                                <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                                <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Cazuela de Mariscos">✨ Maridaje</button>
                            </div>
                            <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                        </div>
                        <!-- Cazuelas de Camarones -->
                        <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcToW1soQAt_FVCudO9VZh12HprLcEycDZJhqw&s?text=Cazuela+de+Camarones" alt="Cazuela de Camarones" class="rounded-lg mb-4 w-full h-auto object-cover">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Cazuelas de Camarones</h3>
                            <div class="text-gray-600 text-left w-full">
                                <p class="mb-1" data-description="Cazuela de Camarones.">Cazuela de Camarones: <span class="text-blue-600 font-bold">$40.000 - $45.000</span></p>
                                <p class="mb-1" data-description="Cazuela Tsunami con Camarón.">Cazuela Tsunami con Camarón: <span class="text-blue-600 font-bold">$50.000</span></p>
                                <p class="mb-1" data-description="Cazuela de Camarones con Langostinos.">Cazuela de Camarones con Langostinos: <span class="text-blue-600 font-bold">$55.000</span></p>
                            </div>
                            <div class="flex space-x-2 mt-4">
                                <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                                <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Cazuela de Camarones">✨ Maridaje</button>
                            </div>
                            <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                        </div>
                    </div>
                </div>

                <!-- Seafood Menu -->
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 mt-16">
                    <!-- Specialty Item 1 -->
                    <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                        <img src="https://lh3.googleusercontent.com/p/AF1QipPQWHqT217eOiaKusGKhdIahcfrJS35ku-Gtxz6=w203-h135-k-no?text=Parrillada" alt="Parrillada Frutos del Mar" class="rounded-lg mb-4 w-full h-auto object-cover">
                        <h3 class="text-2xl font-bold text-gray-900 mb-2">Parrillada Frutos del Mar</h3>
                        <p class="text-gray-600 mb-4" data-description="Una exquisita selección de mariscos a la parrilla, ideal para una persona.">Una exquisita selección de mariscos a la parrilla, ideal para una persona.</p>
                        <span class="text-xl font-bold text-blue-600">$60.000 COP</span>
                        <div class="flex space-x-2 mt-4">
                            <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                            <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Parrillada Frutos del Mar" data-special-pairing="Una refrescante Limonada de Coco, que equilibra perfectamente los sabores intensos de los mariscos.">✨ Maridaje</button>
                        </div>
                        <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                    </div>
                    <!-- Specialty Item 2 -->
                    <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                        <img src="https://lh3.googleusercontent.com/p/AF1QipMiWt_reTS42wvg0T0CSIC5iRbCdP_d9x_2FxaZ=w203?text=Bandeja+Barra+Marina" alt="Bandeja Barra Marina" class="rounded-lg mb-4 w-full h-auto object-cover">
                        <h3 class="text-2xl font-bold text-gray-900 mb-2">Bandeja Barra Marina</h3>
                        <p class="text-gray-600 mb-4" data-description="Una completa combinación de los mejores sabores del mar.">Una completa combinación de los mejores sabores del mar.</p>
                        <span class="text-xl font-bold text-blue-600">$38.000 COP</span>
                        <div class="flex space-x-2 mt-4">
                            <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                            <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Bandeja Barra Marina" data-special-pairing="Una refrescante limonada cítrica, que resalta los sabores frescos del plato.">✨ Maridaje</button>
                        </div>
                        <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                    </div>
                    <!-- New Ceviche de Mariscos Item -->
                    <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRqp7fT_a6bPuNdj2GFjlsyWZwoWd2VXegPxA&stext=Ceviche+Mariscos" alt="Ceviche de Mariscos" class="rounded-lg mb-4 w-full h-auto object-cover">
                        <h3 class="text-2xl font-bold text-gray-900 mb-2">Ceviche de Mariscos</h3>
                        <div class="text-gray-600 text-left w-full">
                            <p class="mb-1" data-description="Ceviche de mariscos de 7 onzas.">7 ONZ: <span class="text-blue-600 font-bold">$17.000 COP</span></p>
                            <p class="mb-1" data-description="Ceviche de mariscos de 16 onzas.">16 ONZ: <span class="text-blue-600 font-bold">$27.000 COP</span></p>
                            <p class="mb-1" data-description="Ceviche de mariscos de 24 onzas.">24 ONZ: <span class="text-blue-600 font-bold">$40.000 COP</span></p>
                            <p class="mb-1" data-description="Ceviche de mariscos y langostinos.">Ceviche de Mariscos y langostinos: <span class="text-blue-600 font-bold">$42.000 COP</span></p>
                        </div>
                        <div class="flex space-x-2 mt-4">
                            <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                            <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Ceviche de Mariscos" data-special-pairing="Una cerveza Coronita, que con su sabor ligero y notas cítricas, realza la frescura del plato.">✨ Maridaje</button>
                        </div>
                        <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                    </div>
                    <!-- New Ceviche de Camarones Item -->
                    <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                        <img src="https://lh3.googleusercontent.com/p/AF1QipMi8hkMMrc-d1Gw5iyyS99sJAk-iqJevk-Ed-dU=w203-h212-k-no?text=Ceviche+Camarones" alt="Ceviche de Camarones" class="rounded-lg mb-4 w-full h-auto object-cover">
                        <h3 class="text-2xl font-bold text-gray-900 mb-2">Ceviche de Camarones</h3>
                        <div class="text-gray-600 text-left w-full">
                            <p class="mb-1" data-description="Ceviche de camarones de 7 onzas.">7 ONZ: <span class="text-blue-600 font-bold">$18.000 COP</span></p>
                            <p class="mb-1" data-description="Ceviche de camarones de 16 onzas.">16 ONZ: <span class="text-blue-600 font-bold">$28.000 COP</span></p>
                            <p class="mb-1" data-description="Ceviche de camarones de 24 onzas.">24 ONZ: <span class="text-blue-600 font-bold">$42.000 COP</span></p>
                            <p class="mb-1" data-description="Ceviche de camarones y langostinos.">Ceviche de Camarón y langostinos: <span class="text-blue-600 font-bold">$45.000 COP</span></p>
                        </div>
                        <div class="flex space-x-2 mt-4">
                            <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                            <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Ceviche de Camarones" data-special-pairing="Una cerveza Coronita, que con su sabor ligero y notas cítricas, realza la frescura del plato.">✨ Maridaje</button>
                        </div>
                        <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                    </div>
                    <!-- Menu Item for Arroz con Camarón -->
                    <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTDwhGVjQVCdMrkRXR5d3Fld3Ok0YV0cLfGeQ&s?text=Arroz+con+Camarón" alt="Arroz con Camarón" class="rounded-lg mb-4 w-full h-auto object-cover">
                        <h3 class="text-2xl font-bold text-gray-900 mb-2">Arroz con Camarón</h3>
                        <p class="text-gray-600 mb-4" data-description="Delicioso arroz  preparado con camarones frescos, vegetales y especias.">Delicioso arroz cremoso preparado con camarones frescos, vegetales y especias.</p>
                        <span class="text-xl font-bold text-blue-600">Entre $35.000 y $40.000 COP</span>
                        <div class="flex space-x-2 mt-4">
                            <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                            <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Arroz con Camarón">✨ Maridaje</button>
                        </div>
                        <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                    </div>
                    <!-- Menu Item 2 -->
                    <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                        <img src="https://lh3.googleusercontent.com/p/AF1QipOolGMGBQFLqEtW6ja52qvFoIcss3IMFMYOA3vI=w243-h304-n-k-no-nu?text=Arroz+Marinera" alt="Arroz a la Marinera" class="rounded-lg mb-4 w-full h-auto object-cover">
                        <h3 class="text-2xl font-bold text-gray-900 mb-2">Arroz a la Marinera</h3>
                        <p class="text-gray-600 mb-4" data-description="Arroz  con camarones, calamares y palmitos.">Arroz  con camarones, calamar, pulpo y palmitos.</p>
                        <span class="text-xl font-bold text-blue-600">Entre 30.000 y 35.000 pesos</span> 
                        <div class="flex space-x-2 mt-4">
                            <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                            <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Arroz a la Marinera">✨ Maridaje</button>
                        </div>
                        <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                    </div>
                    <!-- Menu Item 3 -->
                    <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                        <img src="https://lh3.googleusercontent.com/p/AF1QipMw87E6PyhkVcc1PHNHkXMSlnJD5tOcgWDlvJ1H=w243-h244-n-k-no-nu?text=mojarra" alt="mojarra Frita" class="rounded-lg mb-4 w-full h-auto object-cover">
                        <h3 class="text-2xl font-bold text-gray-900 mb-2">mojarra Frita</h3>
                        <p class="text-gray-600 mb-4" data-description="mojarra roja entera, frita a la perfección, acompañado de patacones.">mojarra roja entera, frita a la perfección, acompañado de patacones.</p>
                        <span class="text-xl font-bold text-blue-600">Según el tamaño</span>
                        <div class="flex space-x-2 mt-4">
                            <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                            <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="mojarra Roja Frito">✨ Maridaje</button>
                        </div>
                        <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                    </div>
                    <!-- Menu Item 4 -->
                    <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                        <img src="https://lh3.googleusercontent.com/p/AF1QipO1UFrtmCRhro-0Ci8VEStjXwF4yiFkgjkHf2jR=s680-w680-h510-rw?text=Pescado+Sierra" alt="Sierra" class="rounded-lg mb-4 w-full h-auto object-cover">
                        <h3 class="text-2xl font-bold text-gray-900 mb-2">Sierra</h3>
                        <p class="text-gray-600 mb-4" data-description="Pescado Sierra fresco frito, acompañado de ensalada y patacones.">Pescado Sierra fresco frito, acompañado de ensalada y patacones.</p>
                        <span class="text-xl font-bold text-blue-600">Según el tamaño</span>
                        <div class="flex space-x-2 mt-4">
                            <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                            <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Pescado Sierra">✨ Maridaje</button>
                        </div>
                        <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                    </div>
                    <!-- New Menu Item for Filete de Pescado Apanado -->
                    <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQG-SGW0_gZ3uhFV-Jh98ruxYQJk7n-ypge4w&s?text=Filete+Apanado" alt="Filete de Pescado Apanado" class="rounded-lg mb-4 w-full h-auto object-cover">
                        <h3 class="text-2xl font-bold text-gray-900 mb-2">Filete de Pescado Apanado</h3>
                        <p class="text-gray-600 mb-4" data-description="Crujiente filete de pescado apanado, servido con ensalada y patacones.">Crujiente filete de pescado apanado, servido con ensalada y patacones.</p>
                        <span class="text-xl font-bold text-blue-600">Desde $18.000 hasta $28.000 COP</span>
                        <div class="flex space-x-2 mt-4">
                            <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                            <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Filete de Pescado Apanado">✨ Maridaje</button>
                        </div>
                        <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                    </div>
                     <!-- New Menu Item for Bagre -->
                    <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQJcWAmGAZ_9sr9EpyuaP9r612CARVk-v_rzw&s?text=Bagre" alt="Bagre Frito o Sudado" class="rounded-lg mb-4 w-full h-auto object-cover">
                        <h3 class="text-2xl font-bold text-gray-900 mb-2">Bagre Frito o Sudado</h3>
                        <p class="text-gray-600 mb-4" data-description="Un filete de bagre fresco, preparado a tu elección: crujiente y dorado, o cocinado lentamente en una salsa especial de la casa. Acompañado de arroz, patacón y ensalada fresca.">Un filete de bagre fresco, preparado a tu elección: crujiente y dorado, o cocinado lentamente en una salsa especial de la casa. Acompañado de arroz, patacón y ensalada fresca.</p>
                        <span class="text-xl font-bold text-blue-600">Desde $20.000 hasta $30.000 COP</span>
                        <div class="flex space-x-2 mt-4">
                            <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                            <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Bagre">✨ Maridaje</button>
                        </div>
                        <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                    </div>
                    <!-- Menu Item for Salmón -->
                    <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                        <img src="https://lh3.googleusercontent.com/gps-cs-s/AC9h4noTbSSx2kws_o8yfoqYFeYETj3w7w8OJqIDbNiU09mpn6e5AXikKkEFFD8TJlFfQQ4LGds-HWq1Dhj0lovuLBuGd0VGEqNYfFz7345ZqYdLViBA8vhHfZD-IchXQmB9HS77cHD54w=s680-w680-h510-rw?text=Salmon+a+la+plancha" alt="Salmón a la plancha" class="rounded-lg mb-4 w-full h-auto object-cover">
                        <h3 class="text-2xl font-bold text-gray-900 mb-2">Salmón</h3>
                        <div class="text-gray-600 text-left w-full">
                            <p class="mb-1" data-description="Salmón a la plancha.">Salmón a la plancha: <span class="text-blue-600 font-bold">$40.000</span></p>
                            <p class="mb-1" data-description="Salmón Gratinado.">Salmón Gratinado: <span class="text-blue-600 font-bold">$45.000</span></p>
                            <p class="mb-1" data-description="Salmón en salsa de Maracuyá o al Ajillo.">Salmón en salsa de Maracuyá o al Ajillo: <span class="text-blue-600 font-bold">$45.000</span></p>
                            <p class="mb-1" data-description="Salmón a la marinera o en Salsa de Camarón.">Salmón a la marinera o en Salsa de Camarón: <span class="text-blue-600 font-bold">$50.000</span></p>
                        </div>
                        <div class="flex space-x-2 mt-4">
                            <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                            <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Salmón">✨ Maridaje</button>
                        </div>
                        <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                    </div>
                    <!-- Menu Item for Paellas -->
                    <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                        <img src="https://lh3.googleusercontent.com/gps-cs-s/AC9h4nrUcSLicOPT0Q2jrC1DAvmChFJ12lrOEkOV6WmWnGhsj7SiFAGJwfSN7fBN-8EKFYV7e_dpMjHc0_gIxS1w_ByqAbrIJz8VNNlnIxiyp8CtIZl00PNWLJZMo8KtmjzU-3_3mR1Bug=w243-h174-n-k-no-nu?text=Paella" alt="Paella" class="rounded-lg mb-4 w-full h-auto object-cover">
                        <h3 class="text-2xl font-bold text-gray-900 mb-2">Paellas</h3>
                        <div class="text-gray-600 text-left w-full">
                            <p class="mb-1" data-description="Paella Valenciana con mariscos y carnes.">Paella Valenciana (Mariscos y carnes): <span class="text-blue-600 font-bold">$45.000</span></p>
                            <p class="mb-1" data-description="Paella Marinera personal con Langostinos.">Paella Marinera personal con Langostinos: <span class="text-blue-600 font-bold">$50.000</span></p>
                        </div>
                        <div class="flex space-x-2 mt-4">
                            <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                            <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Paella">✨ Maridaje</button>
                        </div>
                        <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                    </div>
                    <!-- New Menu Item for Trucha -->
                    <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                        <img src="https://lh3.googleusercontent.com/p/AF1QipPTrnw_XGZTVa7y9PirfnecMJcxeY0mTKSmDXlG=w243-h244-n-k-no-nu?text=Trucha" alt="Trucha a la plancha" class="rounded-lg mb-4 w-full h-auto object-cover">
                        <h3 class="text-2xl font-bold text-gray-900 mb-2">Trucha</h3>
                        <div class="text-gray-600 text-left w-full">
                            <p class="mb-1" data-description="Trucha a la plancha.">Trucha a la plancha: <span class="text-blue-600 font-bold">Entre $30.000 y $35.000 COP</span></p>
                            <p class="mb-1" data-description="Trucha gratinada.">Trucha gratinada: <span class="text-blue-600 font-bold">Entre $35.000 y $40.000 COP</span></p>
                            <p class="mb-1" data-description="Trucha en salsa de Maracuyá o al Ajillo.">Trucha en salsa de Maracuyá o al Ajillo: <span class="text-blue-600 font-bold">Entre $35.000 y $40.000 COP</span></p>
                            <p class="mb-1" data-description="Trucha a la marinera o en Salsa de Camarón.">Trucha a la marinera o en Salsa de Camarón: <span class="text-blue-600 font-bold">Entre $40.000 y $45.000 COP</span></p>
                        </div>
                        <div class="flex space-x-2 mt-4">
                            <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                            <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Trucha">✨ Maridaje</button>
                        </div>
                        <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                    </div>
                    <!-- Menu Item for Pasta -->
                    <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                        <img src="https://lh3.googleusercontent.com/p/AF1QipN0mv9BPpoynqT48yTH6AGDafHjf2FDGIQXqhf6=s426-k-?text=Pasta" alt="Pasta a la marinera" class="rounded-lg mb-4 w-full h-auto object-cover">
                        <h3 class="text-2xl font-bold text-gray-900 mb-2">Pastas</h3>
                        <div class="text-gray-600 text-left w-full">
                            <p class="mb-1" data-description="Pastas a la marinera.">Pastas a la marinera: <span class="text-blue-600 font-bold">30.000 - 35.000</span></p>
                            <p class="mb-1" data-description="Pastas con Camarones.">Pastas con Camarones: <span class="text-blue-600 font-bold">35.000 - 40.000</span></p>
                        </div>
                        <div class="flex space-x-2 mt-4">
                            <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                            <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Pasta">✨ Maridaje</button>
                        </div>
                        <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                    </div>
                    <!-- Menu Item for Langostinos -->
                    <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR1gNkC4pqH3UHrWsAwHlN5tYLsKzgdeYms2w&s?text=Langostinos" alt="Langostinos apanados" class="rounded-lg mb-4 w-full h-auto object-cover">
                        <h3 class="text-2xl font-bold text-gray-900 mb-2">Langostinos</h3>
                        <p class="text-gray-600 mb-4" data-description="8 unidades de langostinos apanados o al ajillo.">8 unidades de langostinos apanados o al ajillo.</p>
                        <span class="text-xl font-bold text-blue-600">60.000 pesos</span>
                        <div class="flex space-x-2 mt-4">
                            <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                            <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Langostinos">✨ Maridaje</button>
                        </div>
                        <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                    </div>
                    <!-- Menu Item for Patacon -->
                    <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRbGMNZj1LKsVK5D-mqJmIlmNdyGsR84VSr8Q&s?text=Patacon" alt="Patacón a la Marinera" class="rounded-lg mb-4 w-full h-auto object-cover">
                        <h3 class="text-2xl font-bold text-gray-900 mb-2">Patacón</h3>
                        <p class="text-gray-600 mb-4" data-description="Patacón a la marinera o en salsa de camarones.">Patacón a la marinera o en salsa de camarones.</p>
                        <span class="text-xl font-bold text-blue-600">30.000 pesos</span>
                        <div class="flex space-x-2 mt-4">
                            <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                            <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Patacón">✨ Maridaje</button>
                        </div>
                        <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                    </div>
                    <!-- New Menu Item for Camarones -->
                    <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                        <img src="https://lh3.googleusercontent.com/p/AF1QipOX8ErAgu-m9zEzR7oLSVQfwE72uSQXOtR75HVW=w203-h135-k-n?text=Camarones" alt="Camarones apanados o al ajillo" class="rounded-lg mb-4 w-full h-auto object-cover">
                        <h3 class="text-2xl font-bold text-gray-900 mb-2">Camarones</h3>
                        <p class="text-gray-600 mb-4" data-description="Camarones apanados o al ajillo.">Camarones apanados o al ajillo.</p>
                        <span class="text-xl font-bold text-blue-600">35.000 pesos</span>
                        <div class="flex space-x-2 mt-4">
                            <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                            <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Camarones">✨ Maridaje</button>
                        </div>
                        <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                    </div>
                </div>

                <!-- New Meats Menu Section -->
                <div class="mt-16 text-center">
                    <h2 class="text-4xl font-bold text-gray-900 mb-8">Línea Especial de Carnes</h2>
                    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                        <!-- Churrasco -->
                        <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTh6xNAju0KHXTowL2p8Fwu4gZ4qBieDgvU5Q&s?text=Churrasco" alt="Churrasco a la plancha" class="rounded-lg mb-4 w-full h-auto object-cover">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Churrasco a la plancha</h3>
                            <p class="text-gray-600 mb-4" data-description="Delicioso churrasco a la parrilla, acompañado de patacones y ensalada.">Delicioso churrasco a la parrilla, acompañado de patacones y ensalada.</p>
                            <span class="text-xl font-bold text-blue-600">32.000 pesos</span>
                            <div class="flex space-x-2 mt-4">
                                <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                                <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Churrasco">✨ Maridaje</button>
                            </div>
                            <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                        </div>
                        <!-- Pechuga a la plancha -->
                        <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcStOuGVxu55uP6rIzFvcD5IRacdGtDNx0MJOg&s ?text=Pechuga+Plancha" alt="Pechuga a la plancha" class="rounded-lg mb-4 w-full h-auto object-cover">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Pechuga a la plancha</h3>
                            <p class="text-gray-600 mb-4" data-description="Jugosa pechuga de pollo a la plancha, servida con papas a la francesa y ensalada.">Jugosa pechuga de pollo a la plancha, servida con papas a la francesa y ensalada.</p>
                            <span class="text-xl font-bold text-blue-600">28.000 pesos</span>
                            <div class="flex space-x-2 mt-4">
                                <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                                <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Pechuga a la plancha">✨ Maridaje</button>
                            </div>
                            <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                        </div>
                        <!-- Pechuga gratinada -->
                        <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTaiBYjnoEEPPmn17gN0lKLR1ew7hK61mZFig&s?text=Pechuga+Gratinada" alt="Pechuga gratinada" class="rounded-lg mb-4 w-full h-auto object-cover">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Pechuga gratinada</h3>
                            <p class="text-gray-600 mb-4" data-description="Pechuga de pollo a la plancha cubierta con una capa de queso gratinado.">Pechuga de pollo a la plancha cubierta con una capa de queso gratinado.</p>
                            <span class="text-xl font-bold text-blue-600">32.000 pesos</span>
                            <div class="flex space-x-2 mt-4">
                                <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                                <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Pechuga gratinada">✨ Maridaje</button>
                            </div>
                            <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                        </div>
                        <!-- Lomo de cerdo -->
                        <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTisYcr5HPPTO4aT_7qnCzHm6v_juoHgkpmgQ&s?text=Lomo+de+Cerdo" alt="Lomo de cerdo a la plancha" class="rounded-lg mb-4 w-full h-auto object-cover">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Lomo de cerdo a la plancha</h3>
                            <p class="text-gray-600 mb-4" data-description="Suave lomo de cerdo a la plancha, servido con arroz y ensalada.">Suave lomo de cerdo a la plancha, servido con arroz y ensalada.</p>
                            <span class="text-xl font-bold text-blue-600">28.000 pesos</span>
                            <div class="flex space-x-2 mt-4">
                                <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                                <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Lomo de cerdo">✨ Maridaje</button>
                            </div>
                            <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                        </div>
                        <!-- Costillas Bbq o Miel Mostaza -->
                        <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS5PBFG0twpqlrrRp_RL8GZaQR6lWFs3yBCuw&s?text=Costillas+BBQ" alt="Costillas BBQ o Miel Mostaza" class="rounded-lg mb-4 w-full h-auto object-cover">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Costillas BBQ o Miel Mostaza</h3>
                            <p class="text-gray-600 mb-4" data-description="Tiernas costillas de cerdo bañadas en salsa BBQ o miel mostaza.">Tiernas costillas de cerdo bañadas en salsa BBQ o miel mostaza.</p>
                            <span class="text-xl font-bold text-blue-600">30.000 pesos</span>
                            <div class="flex space-x-2 mt-4">
                                <button class="speak-button bg-blue-500 text-white py-1 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300">✨ Escuchar</button>
                                <button class="pairing-button bg-purple-500 text-white py-1 px-4 rounded-full text-sm hover:bg-purple-600 transition duration-300" data-dish="Costillas BBQ">✨ Maridaje</button>
                            </div>
                            <div class="pairing-output mt-2 text-gray-500 italic text-sm"></div>
                        </div>
                    </div>
                </div>

                <!-- Kids' Menu Section -->
                <div class="mt-16 text-center">
                    <h2 class="text-4xl font-bold text-gray-900 mb-8">Menú Infantil ✨</h2>
                    <div class="flex flex-col md:flex-row justify-center items-center gap-8">
                        <div class="bg-white rounded-lg shadow-lg p-6 w-full md:w-1/3 text-center transition duration-300 transform hover:scale-105">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSt8Ei2Dvqe4TAkwH059-YGNhXRiaBWHxc4_A&s?text=Nuggets" alt="Nuggets de pollo" class="rounded-lg mb-4 w-full h-auto object-cover">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Nuggets de pollo</h3>
                            <span class="text-xl font-bold text-blue-600">16.000 pesos</span>
                        </div>
                        <div class="bg-white rounded-lg shadow-lg p-6 w-full md:w-1/3 text-center transition duration-300 transform hover:scale-105">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSBHnMJcqxfvmDVfPTHHRgTn4lV6bzbCiRE5w&s?text=Pastas+con+pollo" alt="Pastas con pollo" class="rounded-lg mb-4 w-full h-auto object-cover">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Pastas con pollo</h3>
                            <span class="text-xl font-bold text-blue-600">25.000 pesos</span>
                        </div>
                        <div class="bg-white rounded-lg shadow-lg p-6 w-full md:w-1/3 text-center transition duration-300 transform hover:scale-105">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRd6J3YzSSKpOSb_Efdy_TL9DQSzCZmHe4UNQ&s?text=Arroz+con+pollo" alt="Arroz con pollo" class="rounded-lg mb-4 w-full h-auto object-cover">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Arroz con pollo</h3>
                            <span class="text-xl font-bold text-blue-600">25.000 pesos</span>
                        </div>
                    </div>
                    <!-- Recommended Drinks for Kids -->
                    <div class="mt-8 bg-yellow-100 border-l-4 border-yellow-500 text-yellow-700 p-4 rounded-lg shadow-md">
                        <h4 class="text-xl font-bold mb-2">🥤 Bebidas Recomendadas para Niños</h4>
                        <p>¡Acompaña sus platos favoritos con nuestras bebidas más divertidas y refrescantes!</p>
                        <ul class="list-disc list-inside mt-2 text-left max-w-md mx-auto">
                            <li><strong>Limonada de Coco:</strong> Una cremosa y dulce aventura tropical.</li>
                            <li><strong>Limonada Cerezada:</strong> El toque perfecto de dulzura y color.</li>
                            <li><strong>Malteada de Vainilla:</strong> Cremosa y dulce, ideal para los más pequeños.</li>
                        </ul>
                    </div>
                </div>

                <!-- Drinks Section -->
                <div class="mt-16 text-center">
                    <h2 class="text-4xl font-bold text-gray-900 mb-8">Bebidas ✨</h2>
                    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-8">
                        <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Gaseosa 350 ml.</h3>
                            <span class="text-xl font-bold text-blue-600">3.500 pesos</span>
                        </div>
                        <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Cerveza Nal.</h3>
                            <span class="text-xl font-bold text-blue-600">4.000 pesos</span>
                        </div>
                        <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Gaseosa 1,5 lt.</h3>
                            <span class="text-xl font-bold text-blue-600">9.000 pesos</span>
                        </div>
                        <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Cerveza Coronita</h3>
                            <span class="text-xl font-bold text-blue-600">5.000 pesos</span>
                        </div>
                        <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Agua 600 ml.</h3>
                            <span class="text-xl font-bold text-blue-600">3.000 pesos</span>
                        </div>
                        <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Jugo Natural en Agua</h3>
                            <span class="text-xl font-bold text-blue-600">6.000 pesos</span>
                        </div>
                        <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Jugo Natural en Leche</h3>
                            <span class="text-xl font-bold text-blue-600">7.000 pesos</span>
                        </div>
                        <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Limonada de Coco</h3>
                            <span class="text-xl font-bold text-blue-600">9.000 pesos</span>
                        </div>
                        <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Limonada Cerezada</h3>
                            <span class="text-xl font-bold text-blue-600">9.000 pesos</span>
                        </div>
                        <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col items-center text-center transition duration-300 transform hover:scale-105">
                            <h3 class="text-2xl font-bold text-gray-900 mb-2">Limonada Cítrica</h3>
                            <span class="text-xl font-bold text-blue-600">9.000 pesos</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer Section -->
    <footer class="bg-gray-800 text-white py-12">
        <div class="container mx-auto px-4 text-center">
            <h3 class="text-3xl font-bold mb-4">La Barra Marina</h3>
            <div class="text-lg text-gray-300 mb-4">
                <p>Dirección: Carrera 16 #8-01 Melgar, Tolima 734001, frente al Éxito de Cafam</p>
                <p>Teléfono: +57 312 4832174</p>
                <p>Facebook: <a href="https://www.facebook.com/share/1GYwxkygLi/" target="_blank" class="text-blue-400 hover:underline">La Barra Marina Melgar</a></p>
                <p>WhatsApp: <a href="https://wa.link/fu1vpk" target="_blank" class="text-blue-400 hover:underline">Chatear con nosotros</a></p>
            </div>
            <!-- QR Code Section -->
            <div class="mt-8 flex flex-col md:flex-row justify-center items-center gap-8">
                <div>
                    <p class="text-gray-300 mb-2">Ver el menú completo</p>
                    <div id="menu-qrcode" class="p-2 bg-white rounded-lg shadow-lg"></div>
                </div>
                <div>
                    <p class="text-gray-300 mb-2">Escanea para chatear por WhatsApp</p>
                    <div id="whatsapp-qrcode" class="p-2 bg-white rounded-lg shadow-lg"></div>
                </div>
            </div>
            <p class="text-gray-500 mt-8">&copy; 2024 La Barra Marina. Todos los derechos reservados.</p>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const pairingButtons = document.querySelectorAll('.pairing-button');
            const speakButtons = document.querySelectorAll('.speak-button');
            const searchInput = document.getElementById('searchInput');
            const menuCards = document.querySelectorAll('#menuItemsContainer .bg-white.rounded-lg');

            pairingButtons.forEach(button => {
                button.addEventListener('click', (event) => {
                    const dish = event.target.getAttribute('data-dish');
                    const specialPairing = event.target.getAttribute('data-special-pairing');
                    const outputElement = event.target.closest('div').nextElementSibling;
                    const defaultPairing = `El maridaje ideal para la mayoría de nuestros platos es una cerveza fría o una refrescante limonada.`;

                    if (specialPairing) {
                        outputElement.innerText = specialPairing;
                    } else {
                        outputElement.innerText = defaultPairing;
                    }
                });
            });

            speakButtons.forEach(button => {
                button.addEventListener('click', (event) => {
                    const card = event.target.closest('.bg-white');
                    const dishTitle = card.querySelector('h3').innerText;
                    const dishPrices = Array.from(card.querySelectorAll('.text-blue-600.font-bold')).map(span => span.innerText).join(', ');
                    const dishDescription = card.querySelector('[data-description]')?.getAttribute('data-description') || '';
                    const textToSpeak = `${dishTitle}. ${dishDescription ? dishDescription + '. ' : ''}Precios: ${dishPrices}.`;

                    const utterance = new SpeechSynthesisUtterance(textToSpeak);
                    utterance.lang = 'es-ES';
                    speechSynthesis.speak(utterance);
                });
            });

            searchInput.addEventListener('input', (event) => {
                const searchTerm = event.target.value.toLowerCase();
                menuCards.forEach(card => {
                    const cardText = card.innerText.toLowerCase();
                    if (cardText.includes(searchTerm)) {
                        card.style.display = 'block';
                    } else {
                        card.style.display = 'none';
                    }
                });
            });

            // QR Code Generation
            const whatsappQrCodeElement = document.getElementById('whatsapp-qrcode');
            if (whatsappQrCodeElement) {
                new QRCode(whatsappQrCodeElement, {
                    text: "https://wa.link/fu1vpk",
                    width: 128,
                    height: 128,
                    colorDark: "#000000",
                    colorLight: "#ffffff",
                    correctLevel: QRCode.CorrectLevel.H
                });
            }

            const menuQrCodeElement = document.getElementById('menu-qrcode');
            if (menuQrCodeElement) {
                new QRCode(menuQrCodeElement, {
                    text: window.location.href.split('#')[0] + '#menu',
                    width: 128,
                    height: 128,
                    colorDark: "#000000",
                    colorLight: "#ffffff",
                    correctLevel: QRCode.CorrectLevel.H
                });
            }
        });
    </script>
</body>
</html> 
<!-- Calificación con estrellas y texto -->
<style>
.rating-container {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  margin: 20px 0;
}
.stars {
  display: flex;
  flex-direction: row;
}
.star {
  font-size: 2rem;
  color: #ccc;
  cursor: pointer;
  transition: color 0.2s;
}
.star.selected,
.star:hover,
.star:hover ~ .star {
  color: gold;
}
.rating-text {
  margin-top: 10px;
  width: 300px;
  padding: 6px;
  border: 1px solid #ddd;
  border-radius: 5px;
  font-size: 1rem;
}
.rating-result {
  margin-top: 10px;
  font-style: italic;
  color: #333;
}
</style>

<div class="rating-container">
  <label>Califica este sitio:</label>
  <div class="stars" id="stars">
    <span class="star" data-value="1">&#9733;</span>
    <span class="star" data-value="2">&#9733;</span>
    <span class="star" data-value="3">&#9733;</span>
    <span class="star" data-value="4">&#9733;</span>
    <span class="star" data-value="5">&#9733;</span>
  </div>
  <input type="text" id="ratingText" class="rating-text" placeholder="Escribe tu opinión aquí..." />
  <button onclick="submitRating()">Enviar calificación</button>
  <div id="ratingResult" class="rating-result"></div>
</div>

<script>
const stars = document.querySelectorAll('.star');
let selectedRating = 0;

stars.forEach(star => {
  star.addEventListener('mouseover', function() {
    const val = parseInt(this.getAttribute('data-value'));
    highlightStars(val);
  });
  star.addEventListener('mouseout', function() {
    highlightStars(selectedRating);
  });
  star.addEventListener('click', function() {
    selectedRating = parseInt(this.getAttribute('data-value'));
    highlightStars(selectedRating);
  });
});

function highlightStars(rating) {
  stars.forEach(star => {
    if (parseInt(star.getAttribute('data-value')) <= rating) {
      star.classList.add('selected');
    } else {
      star.classList.remove('selected');
    }
  });
}

function submitRating() {
  const text = document.getElementById('ratingText').value;
  if (selectedRating === 0) {
    alert('Por favor selecciona una calificación de estrellas.');
    return;
  }
  if (text.trim() === '') {
    alert('Por favor escribe tu opinión.');
    return;
  }
  document.getElementById('ratingResult').innerText =
    `¡Gracias por tu calificación de ${selectedRating} estrella${selectedRating > 1 ? 's' : ''}!\nTu opinión: ${text}`;
  // Si quieres guardar en localStorage:
  // localStorage.setItem('siteRating', JSON.stringify({stars: selectedRating, text}));
}
</script>
