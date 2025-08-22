        * {
            font-family: 'Inter', sans-serif;
        }
        
        .gradient-bg {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
        
        .gradient-text {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .card-hover {
            transition: all 0.3s ease;
        }
        
        .card-hover:hover {
            transform: translateY(-8px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
        }
        
        .nav-link {
            position: relative;
            transition: color 0.3s ease;
        }
        
        .nav-link::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -4px;
            left: 0;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            transition: width 0.3s ease;
        }
        
        .nav-link:hover::after {
            width: 100%;
        }
        
        .floating-animation {
            animation: float 6s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
        }
        
        .pulse-animation {
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.7; }
        }
        
        .scroll-smooth {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-gray-50 scroll-smooth">
    <!-- Navigation -->
    <nav class="bg-white shadow-lg fixed w-full top-0 z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <div class="flex items-center">
                    <span class="text-2xl font-bold gradient-text">🌐 Big Daddi AI</span>
                </div>
                <div class="hidden md:block">
                    <div class="ml-10 flex items-baseline space-x-8">
                        <a href="#home" class="nav-link text-gray-700 hover:text-purple-600 px-3 py-2 text-sm font-medium">Home</a>
                        <a href="#about" class="nav-link text-gray-700 hover:text-purple-600 px-3 py-2 text-sm font-medium">About</a>
                        <a href="#services" class="nav-link text-gray-700 hover:text-purple-600 px-3 py-2 text-sm font-medium">Services</a>
                        <a href="#packages" class="nav-link text-gray-700 hover:text-purple-600 px-3 py-2 text-sm font-medium">Packages</a>
                        <a href="#contact" class="nav-link text-gray-700 hover:text-purple-600 px-3 py-2 text-sm font-medium">Contact</a>
                    </div>
                </div>
                <div class="md:hidden">
                    <button id="mobile-menu-btn" class="text-gray-700 hover:text-purple-600 focus:outline-none">
                        <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
                        </svg>
                    </button>
                </div>
            </div>
        </div>
        <!-- Mobile menu -->
        <div id="mobile-menu" class="md:hidden hidden bg-white border-t">
            <div class="px-2 pt-2 pb-3 space-y-1">
                <a href="#home" class="block px-3 py-2 text-gray-700 hover:text-purple-600">Home</a>
                <a href="#about" class="block px-3 py-2 text-gray-700 hover:text-purple-600">About</a>
                <a href="#services" class="block px-3 py-2 text-gray-700 hover:text-purple-600">Services</a>
                <a href="#packages" class="block px-3 py-2 text-gray-700 hover:text-purple-600">Packages</a>
                <a href="#contact" class="block px-3 py-2 text-gray-700 hover:text-purple-600">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="gradient-bg min-h-screen flex items-center justify-center pt-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <div class="floating-animation">
                <h1 class="text-5xl md:text-7xl font-bold text-white mb-6">
                    🌐 Big Daddi AI
                </h1>
                <p class="text-xl md:text-2xl text-white mb-8 max-w-3xl mx-auto">
                    Marketing & AI That Works
                </p>
                <p class="text-lg text-white/90 mb-12 max-w-4xl mx-auto leading-relaxed">
                    Your partner in modern marketing and artificial intelligence solutions. We help businesses grow by combining creative strategies with powerful AI-driven tools to increase sales, boost visibility, and build strong brands.
                </p>
                <div class="space-y-4 sm:space-y-0 sm:space-x-4 sm:flex sm:justify-center">
                    <a href="#services" class="inline-block bg-white text-purple-600 px-8 py-4 rounded-full font-semibold hover:bg-gray-100 transition duration-300 shadow-lg">
                        Explore Services
                    </a>
                    <a href="#contact" class="inline-block border-2 border-white text-white px-8 py-4 rounded-full font-semibold hover:bg-white hover:text-purple-600 transition duration-300">
                        Get Started
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-4xl md:text-5xl font-bold text-gray-900 mb-6">About Us</h2>
                <div class="w-24 h-1 gradient-bg mx-auto mb-8"></div>
            </div>
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <div>
                    <h3 class="text-2xl font-bold text-gray-900 mb-6">Every business deserves big results</h3>
                    <p class="text-lg text-gray-600 mb-6 leading-relaxed">
                        At Big Daddi AI, we believe every business deserves big results. Our team blends creativity, strategy, and AI technology to deliver marketing campaigns that stand out and get results.
                    </p>
                    <p class="text-lg text-gray-600 leading-relaxed">
                        We keep things simple, clear, and effective — no fluff, just impact.
                    </p>
                </div>
                <div class="text-center">
                    <div class="inline-block p-8 bg-gradient-to-br from-purple-100 to-blue-100 rounded-3xl">
                        <div class="text-6xl mb-4">🚀</div>
                        <h4 class="text-xl font-semibold text-gray-900 mb-2">Innovation Driven</h4>
                        <p class="text-gray-600">Combining creativity with cutting-edge AI technology</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-4xl md:text-5xl font-bold text-gray-900 mb-6">Our Services</h2>
                <div class="w-24 h-1 gradient-bg mx-auto mb-8"></div>
                <p class="text-xl text-gray-600 max-w-3xl mx-auto">We specialize in comprehensive solutions that drive growth</p>
            </div>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Service 1 -->
                <div class="bg-white p-8 rounded-2xl shadow-lg card-hover">
                    <div class="text-4xl mb-4">🤖</div>
                    <h3 class="text-xl font-bold text-gray-900 mb-4">AI-Powered Marketing</h3>
                    <p class="text-gray-600 leading-relaxed">Smarter targeting, data-driven insights, and automation that saves you time while driving results.</p>
                </div>
                
                <!-- Service 2 -->
                <div class="bg-white p-8 rounded-2xl shadow-lg card-hover">
                    <div class="text-4xl mb-4">📱</div>
                    <h3 class="text-xl font-bold text-gray-900 mb-4">Social Media Management</h3>
                    <p class="text-gray-600 leading-relaxed">Strategy, content creation, scheduling, and engagement to grow your brand online.</p>
                </div>
                
                <!-- Service 3 -->
                <div class="bg-white p-8 rounded-2xl shadow-lg card-hover">
                    <div class="text-4xl mb-4">🎥</div>
                    <h3 class="text-xl font-bold text-gray-900 mb-4">Content Creation & UGC</h3>
                    <p class="text-gray-600 leading-relaxed">Authentic video & photo content that connects with audiences and builds trust.</p>
                </div>
                
                <!-- Service 4 -->
                <div class="bg-white p-8 rounded-2xl shadow-lg card-hover">
                    <div class="text-4xl mb-4">🎨</div>
                    <h3 class="text-xl font-bold text-gray-900 mb-4">Web Design & Branding</h3>
                    <p class="text-gray-600 leading-relaxed">Modern websites, logos, and branding materials that make your business stand out.</p>
                </div>
                
                <!-- Service 5 -->
                <div class="bg-white p-8 rounded-2xl shadow-lg card-hover">
                    <div class="text-4xl mb-4">📈</div>
                    <h3 class="text-xl font-bold text-gray-900 mb-4">Sales Growth Strategies</h3>
                    <p class="text-gray-600 leading-relaxed">Campaigns designed to bring in leads, convert them, and keep your business thriving.</p>
                </div>
                
                <!-- Why Choose Us -->
                <div class="bg-gradient-to-br from-purple-600 to-blue-600 p-8 rounded-2xl shadow-lg card-hover text-white">
                    <div class="text-4xl mb-4">⭐</div>
                    <h3 class="text-xl font-bold mb-4">Why Choose Big Daddi AI?</h3>
                    <ul class="space-y-2 text-sm">
                        <li>✅ Creative + AI-driven strategies</li>
                        <li>✅ Affordable packages for every business size</li>
                        <li>✅ Hands-on support and personal attention</li>
                        <li>✅ Fresh ideas that work in today's fast-paced world</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Packages Section -->
    <section id="packages" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-4xl md:text-5xl font-bold text-gray-900 mb-6">Packages & Specials</h2>
                <div class="w-24 h-1 gradient-bg mx-auto mb-8"></div>
                <p class="text-xl text-gray-600">Choose the perfect package for your business needs</p>
            </div>
            <div class="grid md:grid-cols-3 gap-8">
                <!-- Starter Package -->
                <div class="bg-white border-2 border-gray-200 p-8 rounded-2xl shadow-lg card-hover">
                    <div class="text-center">
                        <div class="text-4xl mb-4">🎯</div>
                        <h3 class="text-2xl font-bold text-gray-900 mb-2">Starter Marketing Package</h3>
                        <p class="text-gray-600 mb-6">Perfect for small businesses getting online</p>
                        <a href="#contact" class="inline-block bg-gray-900 text-white px-6 py-3 rounded-full font-semibold hover:bg-gray-800 transition duration-300">
                            Learn More
                        </a>
                    </div>
                </div>
                
                <!-- Growth Package -->
                <div class="bg-gradient-to-br from-purple-600 to-blue-600 p-8 rounded-2xl shadow-lg card-hover text-white transform scale-105">
                    <div class="text-center">
                        <div class="text-4xl mb-4">🚀</div>
                        <h3 class="text-2xl font-bold mb-2">Growth Package</h3>
                        <p class="text-white/90 mb-6">Social media + AI insights + lead generation</p>
                        <div class="bg-white/20 text-xs px-3 py-1 rounded-full mb-4 inline-block pulse-animation">
                            MOST POPULAR
                        </div>
                        <a href="#contact" class="inline-block bg-white text-purple-600 px-6 py-3 rounded-full font-semibold hover:bg-gray-100 transition duration-300">
                            Get Started
                        </a>
                    </div>
                </div>
                
                <!-- Elite Package -->
                <div class="bg-white border-2 border-gray-200 p-8 rounded-2xl shadow-lg card-hover">
                    <div class="text-center">
                        <div class="text-4xl mb-4">🏆</div>
                        <h3 class="text-2xl font-bold text-gray-900 mb-2">Elite Package</h3>
                        <p class="text-gray-600 mb-6">Full marketing suite with strategy, branding, and content</p>
                        <a href="#contact" class="inline-block bg-gray-900 text-white px-6 py-3 rounded-full font-semibold hover:bg-gray-800 transition duration-300">
                            Learn More
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-4xl md:text-5xl font-bold text-gray-900 mb-6">Contact Us</h2>
                <div class="w-24 h-1 gradient-bg mx-auto mb-8"></div>
                <p class="text-xl text-gray-600">Let's chat about your business goals</p>
            </div>
            <div class="grid md:grid-cols-2 gap-12">
                <!-- Contact Info -->
                <div class="space-y-8">
                    <div class="flex items-center space-x-4">
                        <div class="bg-purple-100 p-3 rounded-full">
                            <svg class="w-6 h-6 text-purple-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"></path>
                            </svg>
                        </div>
                        <div>
                            <h3 class="font-semibold text-gray-900">Phone</h3>
                            <p class="text-gray-600">084 263 9491</p>
                        </div>
                    </div>
                    
                    <div class="flex items-center space-x-4">
                        <div class="bg-purple-100 p-3 rounded-full">
                            <svg class="w-6 h-6 text-purple-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 4.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path>
                            </svg>
                        </div>
                        <div>
                            <h3 class="font-semibold text-gray-900">Email</h3>
                            <p class="text-gray-600">bigdaddi.aiservices@gmail.com</p>
                        </div>
                    </div>
                    
                    <!-- Social Media -->
                    <div>
                        <h3 class="font-semibold text-gray-900 mb-4">Follow Us</h3>
                        <div class="flex space-x-4">
                            <a href="https://www.facebook.com/share/16pxjZsuXo/" target="_blank" class="bg-blue-600 text-white p-3 rounded-full hover:bg-blue-700 transition duration-300">
                                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M24 12.073c0-6.627-5.373-12-12-12s-12 5.373-12 12c0 5.99 4.388 10.954 10.125 11.854v-8.385H7.078v-3.47h3.047V9.43c0-3.007 1.792-4.669 4.533-4.669 1.312 0 2.686.235 2.686.235v2.953H15.83c-1.491 0-1.956.925-1.956 1.874v2.25h3.328l-.532 3.47h-2.796v8.385C19.612 23.027 24 18.062 24 12.073z"/>
                                </svg>
                            </a>
                            <a href="https://www.instagram.com/bigdaddiai?igsh=dWEwb3RidXRweXkz" target="_blank" class="bg-pink-600 text-white p-3 rounded-full hover:bg-pink-700 transition duration-300">
                                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M12.017 0C5.396 0 .029 5.367.029 11.987c0 6.62 5.367 11.987 11.988 11.987 6.62 0 11.987-5.367 11.987-11.987C24.014 5.367 18.637.001 12.017.001zM8.449 16.988c-1.297 0-2.448-.49-3.323-1.297C4.198 14.895 3.708 13.744 3.708 12.447s.49-2.448 1.297-3.323C5.902 8.198 7.053 7.708 8.35 7.708s2.448.49 3.323 1.297c.897.875 1.387 2.026 1.387 3.323s-.49 2.448-1.297 3.323c-.875.897-2.026 1.387-3.323 1.387z"/>
                                </svg>
                            </a>
                            <a href="https://www.tiktok.com/@bigdaddiai?_t=ZS-8z5X7cFfjfz&_r=1" target="_blank" class="bg-black text-white p-3 rounded-full hover:bg-gray-800 transition duration-300">
                                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M19.59 6.69a4.83 4.83 0 01-3.77-4.25V2h-3.45v13.67a2.89 2.89 0 01-5.2 1.74 2.89 2.89 0 012.31-4.64 2.93 2.93 0 01.88.13V9.4a6.84 6.84 0 00-.88-.05A6.33 6.33 0 005 20.1a6.34 6.34 0 0010.86-4.43v-7a8.16 8.16 0 004.77 1.52v-3.4a4.85 4.85 0 01-1-.1z"/>
                                </svg>
                            </a>
                        </div>
                    </div>
                </div>
                
                <!-- Contact Form -->
                <div class="bg-white p-8 rounded-2xl shadow-lg">
                    <h3 class="text-2xl font-bold text-gray-900 mb-6">Send us a message</h3>
                    <form class="space-y-6">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Name</label>
                            <input type="text" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-purple-500 focus:border-transparent" placeholder="Your name">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Email</label>
                            <input type="email" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-purple-500 focus:border-transparent" placeholder="your@email.com">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Message</label>
                            <textarea rows="4" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-purple-500 focus:border-transparent" placeholder="Tell us about your business goals..."></textarea>
                        </div>
                        <button type="submit" class="w-full gradient-bg text-white py-3 rounded-lg font-semibold hover:opacity-90 transition duration-300">
                            Send Message
                        </button>
                    </form>
                    <p class="text-sm text-gray-500 mt-4 text-center">This is a demo form. Please use the contact information above to reach us.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <div class="mb-8">
                <h3 class="text-3xl font-bold gradient-text mb-4">✨ Big Daddi AI</h3>
                <p class="text-xl text-gray-300">Where Big Ideas Meet AI Power</p>
            </div>
            <div class="border-t border-gray-800 pt-8">
                <p class="text-gray-400">&copy; 2024 Big Daddi AI. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        
        mobileMenuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });
        
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                    // Close mobile menu if open
                    mobileMenu.classList.add('hidden');
                }
            });
        });
        
        // Contact form submission
        document.querySelector('form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Thank you for your message! Please use our contact information above to reach us directly.');
        });
        
        // Add scroll effect to navigation
        window.addEventListener('scroll', () => {
            const nav = document.querySelector('nav');
            if (window.scrollY > 100) {
                nav.classList.add('bg-white/95', 'backdrop-blur-sm');
            } else {
                nav.classList.remove('bg-white/95', 'backdrop-blur-sm');
            }
        });
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'9731ef8965d8881b',t:'MTc1NTg2MTE1Mi4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
