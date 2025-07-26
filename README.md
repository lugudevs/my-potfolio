<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jamilu Abubakar - Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
        body { font-family: 'Inter', sans-serif; }
        
        .gradient-bg {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
        
        .card-hover {
            transition: all 0.3s ease;
        }
        
        .card-hover:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
        }
        
        .skill-bar {
            height: 8px;
            background: linear-gradient(90deg, #667eea, #764ba2);
            border-radius: 4px;
            animation: fillBar 2s ease-in-out;
        }
        
        @keyframes fillBar {
            from { width: 0%; }
        }
        
        .floating {
            animation: float 6s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
        }
    </style>
</head>
<body class="bg-gray-50">
    <!-- Navigation -->
    <nav class="fixed w-full top-0 z-50 bg-white/90 backdrop-blur-md shadow-sm">
        <div class="max-w-6xl mx-auto px-6 py-4">
            <div class="flex justify-between items-center">
                <div class="text-2xl font-bold text-gray-800">JA</div>
                <div class="hidden md:flex space-x-8">
                    <a href="#home" class="text-gray-600 hover:text-purple-600 transition-colors">Home</a>
                    <a href="#about" class="text-gray-600 hover:text-purple-600 transition-colors">About</a>
                    <a href="#services" class="text-gray-600 hover:text-purple-600 transition-colors">Services</a>
                    <a href="#portfolio" class="text-gray-600 hover:text-purple-600 transition-colors">Portfolio</a>
                    <a href="#contact" class="text-gray-600 hover:text-purple-600 transition-colors">Contact</a>
                </div>
                <button class="md:hidden text-gray-600">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                    </svg>
                </button>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="gradient-bg min-h-screen flex items-center pt-20">
        <div class="max-w-6xl mx-auto px-6 text-center text-white">
            <div class="floating mb-8">
                <div class="w-32 h-32 mx-auto bg-white/20 rounded-full flex items-center justify-center backdrop-blur-sm">
                    <span class="text-4xl font-bold">JA</span>
                </div>
            </div>
            <h1 class="text-5xl md:text-7xl font-bold mb-6">Jamilu Abubakar</h1>
            <p class="text-xl md:text-2xl mb-8 opacity-90">Graphic Designer • Web Developer • Tailor</p>
            <p class="text-lg mb-12 max-w-2xl mx-auto opacity-80">Creating beautiful designs, building amazing websites, and crafting perfect fits. Your vision, brought to life with creativity and precision.</p>
            <div class="flex flex-col sm:flex-row gap-4 justify-center">
                <a href="#portfolio" class="bg-white text-purple-600 px-8 py-4 rounded-full font-semibold hover:bg-gray-100 transition-colors">View My Work</a>
                <a href="#contact" class="border-2 border-white text-white px-8 py-4 rounded-full font-semibold hover:bg-white hover:text-purple-600 transition-colors">Get In Touch</a>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 bg-white">
        <div class="max-w-6xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">About Me</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">Passionate creative professional with expertise across multiple disciplines</p>
            </div>
            
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <div>
                    <h3 class="text-2xl font-semibold text-gray-800 mb-6">My Story</h3>
                    <p class="text-gray-600 mb-6">I'm a multi-talented creative professional who believes in the power of good design and craftsmanship. Whether I'm designing a logo, building a website, or tailoring a perfect suit, I bring the same attention to detail and passion for excellence to every project.</p>
                    <p class="text-gray-600 mb-8">My diverse skill set allows me to offer comprehensive solutions to my clients, from digital presence to physical craftsmanship.</p>
                    
                    <div class="space-y-6">
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="font-medium text-gray-700">Graphic Design</span>
                                <span class="text-purple-600">95%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-2">
                                <div class="skill-bar rounded-full" style="width: 95%"></div>
                            </div>
                        </div>
                        
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="font-medium text-gray-700">Web Development</span>
                                <span class="text-purple-600">90%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-2">
                                <div class="skill-bar rounded-full" style="width: 90%"></div>
                            </div>
                        </div>
                        
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="font-medium text-gray-700">Tailoring</span>
                                <span class="text-purple-600">88%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-2">
                                <div class="skill-bar rounded-full" style="width: 88%"></div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="bg-gradient-to-br from-purple-100 to-blue-100 p-8 rounded-2xl">
                    <div class="text-center">
                        <div class="w-24 h-24 mx-auto bg-gradient-to-r from-purple-500 to-blue-500 rounded-full flex items-center justify-center mb-6">
                            <span class="text-2xl">🎨</span>
                        </div>
                        <h4 class="text-xl font-semibold text-gray-800 mb-4">Creative Excellence</h4>
                        <p class="text-gray-600">Combining artistic vision with technical expertise to deliver outstanding results across all creative disciplines.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-20 bg-gray-50">
        <div class="max-w-6xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">My Services</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">Comprehensive creative solutions tailored to your needs</p>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8">
                <div class="bg-white p-8 rounded-2xl shadow-sm card-hover">
                    <div class="w-16 h-16 bg-gradient-to-r from-pink-500 to-rose-500 rounded-xl flex items-center justify-center mb-6">
                        <span class="text-2xl">🎨</span>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-4">Graphic Design</h3>
                    <p class="text-gray-600 mb-6">Logo design, branding, print materials, digital graphics, and visual identity solutions that make your brand stand out.</p>
                    <ul class="text-sm text-gray-500 space-y-2">
                        <li>• Logo & Brand Identity</li>
                        <li>• Print Design</li>
                        <li>• Digital Graphics</li>
                        <li>• Marketing Materials</li>
                    </ul>
                </div>
                
                <div class="bg-white p-8 rounded-2xl shadow-sm card-hover">
                    <div class="w-16 h-16 bg-gradient-to-r from-blue-500 to-cyan-500 rounded-xl flex items-center justify-center mb-6">
                        <span class="text-2xl">💻</span>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-4">Web Development</h3>
                    <p class="text-gray-600 mb-6">Modern, responsive websites and web applications built with the latest technologies and best practices.</p>
                    <ul class="text-sm text-gray-500 space-y-2">
                        <li>• Responsive Websites</li>
                        <li>• E-commerce Solutions</li>
                        <li>• Web Applications</li>
                        <li>• Website Maintenance</li>
                    </ul>
                </div>
                
                <div class="bg-white p-8 rounded-2xl shadow-sm card-hover">
                    <div class="w-16 h-16 bg-gradient-to-r from-purple-500 to-indigo-500 rounded-xl flex items-center justify-center mb-6">
                        <span class="text-2xl">✂️</span>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-4">Tailoring</h3>
                    <p class="text-gray-600 mb-6">Custom clothing, alterations, and bespoke tailoring services with attention to fit, style, and quality craftsmanship.</p>
                    <ul class="text-sm text-gray-500 space-y-2">
                        <li>• Custom Suits</li>
                        <li>• Alterations</li>
                        <li>• Traditional Wear</li>
                        <li>• Repairs & Adjustments</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Portfolio Section -->
    <section id="portfolio" class="py-20 bg-white">
        <div class="max-w-6xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">My Portfolio</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">A showcase of my recent work across different disciplines</p>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="group cursor-pointer">
                    <div class="bg-gradient-to-br from-pink-400 to-purple-600 rounded-2xl p-8 text-white card-hover">
                        <div class="text-4xl mb-4">🎨</div>
                        <h3 class="text-xl font-semibold mb-2">Brand Identity Design</h3>
                        <p class="text-pink-100">Complete branding package for local business</p>
                    </div>
                </div>
                
                <div class="group cursor-pointer">
                    <div class="bg-gradient-to-br from-blue-400 to-cyan-600 rounded-2xl p-8 text-white card-hover">
                        <div class="text-4xl mb-4">💻</div>
                        <h3 class="text-xl font-semibold mb-2">E-commerce Website</h3>
                        <p class="text-blue-100">Modern online store with payment integration</p>
                    </div>
                </div>
                
                <div class="group cursor-pointer">
                    <div class="bg-gradient-to-br from-purple-400 to-indigo-600 rounded-2xl p-8 text-white card-hover">
                        <div class="text-4xl mb-4">✂️</div>
                        <h3 class="text-xl font-semibold mb-2">Custom Suit Collection</h3>
                        <p class="text-purple-100">Bespoke tailoring for special occasions</p>
                    </div>
                </div>
                
                <div class="group cursor-pointer">
                    <div class="bg-gradient-to-br from-green-400 to-teal-600 rounded-2xl p-8 text-white card-hover">
                        <div class="text-4xl mb-4">📱</div>
                        <h3 class="text-xl font-semibold mb-2">Mobile App Design</h3>
                        <p class="text-green-100">UI/UX design for mobile application</p>
                    </div>
                </div>
                
                <div class="group cursor-pointer">
                    <div class="bg-gradient-to-br from-orange-400 to-red-600 rounded-2xl p-8 text-white card-hover">
                        <div class="text-4xl mb-4">📄</div>
                        <h3 class="text-xl font-semibold mb-2">Print Materials</h3>
                        <p class="text-orange-100">Brochures, flyers, and marketing collateral</p>
                    </div>
                </div>
                
                <div class="group cursor-pointer">
                    <div class="bg-gradient-to-br from-violet-400 to-purple-600 rounded-2xl p-8 text-white card-hover">
                        <div class="text-4xl mb-4">👔</div>
                        <h3 class="text-xl font-semibold mb-2">Traditional Wear</h3>
                        <p class="text-violet-100">Custom traditional clothing and alterations</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 gradient-bg text-white">
        <div class="max-w-6xl mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-bold mb-4">Let's Work Together</h2>
                <p class="text-xl opacity-90 max-w-2xl mx-auto">Ready to bring your vision to life? Get in touch and let's discuss your project.</p>
            </div>
            
            <div class="grid md:grid-cols-2 gap-12">
                <div>
                    <h3 class="text-2xl font-semibold mb-8">Get In Touch</h3>
                    
                    <div class="space-y-6">
                        <div class="flex items-center space-x-4">
                            <div class="w-12 h-12 bg-white/20 rounded-full flex items-center justify-center">
                                <span class="text-xl">📧</span>
                            </div>
                            <div>
                                <p class="font-medium">Email</p>
                                <a href="mailto:jermilulugu@gmail.com" class="text-white/80 hover:text-white transition-colors">jermilulugu@gmail.com</a>
                            </div>
                        </div>
                        
                        <div class="flex items-center space-x-4">
                            <div class="w-12 h-12 bg-white/20 rounded-full flex items-center justify-center">
                                <span class="text-xl">📱</span>
                            </div>
                            <div>
                                <p class="font-medium">Phone</p>
                                <a href="tel:09126269104" class="text-white/80 hover:text-white transition-colors">09126269104</a>
                            </div>
                        </div>
                        
                        <div class="flex items-center space-x-4">
                            <div class="w-12 h-12 bg-white/20 rounded-full flex items-center justify-center">
                                <span class="text-xl">💼</span>
                            </div>
                            <div>
                                <p class="font-medium">Services</p>
                                <p class="text-white/80">Design • Development • Tailoring</p>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="bg-white/10 backdrop-blur-sm rounded-2xl p-8">
                    <form class="space-y-6">
                        <div>
                            <label class="block text-sm font-medium mb-2">Name</label>
                            <input type="text" class="w-full px-4 py-3 bg-white/20 border border-white/30 rounded-lg text-white placeholder-white/60 focus:outline-none focus:border-white/60" placeholder="Your Name">
                        </div>
                        
                        <div>
                            <label class="block text-sm font-medium mb-2">Email</label>
                            <input type="email" class="w-full px-4 py-3 bg-white/20 border border-white/30 rounded-lg text-white placeholder-white/60 focus:outline-none focus:border-white/60" placeholder="your@email.com">
                        </div>
                        
                        <div>
                            <label class="block text-sm font-medium mb-2">Service Needed</label>
                            <select class="w-full px-4 py-3 bg-white/20 border border-white/30 rounded-lg text-white focus:outline-none focus:border-white/60">
                                <option value="">Select a service</option>
                                <option value="graphic-design">Graphic Design</option>
                                <option value="web-development">Web Development</option>
                                <option value="tailoring">Tailoring</option>
                                <option value="multiple">Multiple Services</option>
                            </select>
                        </div>
                        
                        <div>
                            <label class="block text-sm font-medium mb-2">Message</label>
                            <textarea rows="4" class="w-full px-4 py-3 bg-white/20 border border-white/30 rounded-lg text-white placeholder-white/60 focus:outline-none focus:border-white/60" placeholder="Tell me about your project..."></textarea>
                        </div>
                        
                        <button type="submit" class="w-full bg-white text-purple-600 py-3 rounded-lg font-semibold hover:bg-gray-100 transition-colors">Send Message</button>
                    </form>
                    
                    <div class="mt-6 p-4 bg-yellow-500/20 border border-yellow-400/30 rounded-lg">
                        <p class="text-sm text-yellow-100">
                            <strong>Demo Form:</strong> This contact form is for display purposes. Please use the email or phone number above to get in touch.
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
        <div class="max-w-6xl mx-auto px-6 text-center">
            <div class="text-2xl font-bold mb-4">Jamilu Abubakar</div>
            <p class="text-gray-400 mb-8">Graphic Designer • Web Developer • Tailor</p>
            <div class="flex justify-center space-x-6 mb-8">
                <a href="mailto:jermilulugu@gmail.com" class="text-gray-400 hover:text-white transition-colors">Email</a>
                <a href="tel:09126269104" class="text-gray-400 hover:text-white transition-colors">Phone</a>
            </div>
            <p class="text-gray-500 text-sm">© 2024 Jamilu Abubakar. All rights reserved.</p>
        </div>
    </footer>

    <script>
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
                }
            });
        });

        // Form submission handler
        document.querySelector('form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Thank you for your message! This is a demo form. Please contact me directly via email or phone.');
        });

        // Add scroll effect to navigation
        window.addEventListener('scroll', function() {
            const nav = document.querySelector('nav');
            if (window.scrollY > 100) {
                nav.classList.add('bg-white/95');
            } else {
                nav.classList.remove('bg-white/95');
            }
        });
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'964cc9ce054cd1fe',t:'MTc1MzQ1ODM2Ny4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
