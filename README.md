!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vismotion | Cinematic Video Editing</title>
    <link rel="stylesheet" href="style.css">
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://unpkg.com/feather-icons"></script>
    <script src="https://cdn.jsdelivr.net/npm/feather-icons/dist/feather.min.js"></script>
    <script>
      tailwind.config = {
        theme: {
          extend: {
            colors: {
              primary: '#0a0a0a',
              secondary: '#1a1a1a',
              accent: '#ffffff'
            },
            animation: {
              'fade-in': 'fadeIn 0.8s ease-in-out',
              'float': 'float 6s ease-in-out infinite',
              'slide-up': 'slideUp 0.6s ease-out'
            },
            keyframes: {
              fadeIn: {
                '0%': { opacity: '0' },
                '100%': { opacity: '1' }
              },
              float: {
                '0%, 100%': { transform: 'translateY(0)' },
                '50%': { transform: 'translateY(-20px)' }
              },
              slideUp: {
                '0%': { transform: 'translateY(40px)', opacity: '0' },
                '100%': { transform: 'translateY(0)', opacity: '1' }
              }
            }
          }
        }
      }
    </script>
</head>
<body class="bg-primary text-accent font-sans antialiased overflow-x-hidden">
    <custom-navbar></custom-navbar>
    
    <main>
        <!-- Hero Section -->
        <section class="relative h-screen flex items-center justify-center overflow-hidden">
            <div class="absolute inset-0 bg-black/60 z-10"></div>
            <video autoplay muted loop class="absolute min-w-full min-h-full object-cover">
                <source src="https://assets.mixkit.co/videos/preview/mixkit-woman-dancing-under-neon-lights-1230-large.mp4" type="video/mp4">
            </video>
            <div class="container mx-auto px-6 relative z-20 text-center animate-fade-in">
                <h1 class="text-5xl md:text-7xl font-bold mb-6 animate-slide-up">VIS<span class="text-accent">MOTION</span></h1>
                <p class="text-xl md:text-2xl max-w-2xl mx-auto mb-8 animate-slide-up delay-100">Cinematic storytelling through motion</p>
                <a href="#portfolio" class="inline-block bg-accent text-primary px-8 py-3 rounded-full font-medium hover:bg-opacity-90 transition-all animate-slide-up delay-200">View Portfolio</a>
            </div>
            <div class="absolute bottom-10 left-1/2 transform -translate-x-1/2 z-20 animate-bounce">
                <i data-feather="chevron-down" class="w-8 h-8"></i>
            </div>
        </section>

        <!-- About Section -->
        <section class="py-20 bg-secondary">
            <div class="container mx-auto px-6">
                <div class="flex flex-col md:flex-row items-center gap-12">
                    <div class="md:w-1/2 animate-slide-up">
                        <h2 class="text-3xl md:text-4xl font-bold mb-6">Crafting Visual <span class="text-accent">Experiences</span></h2>
                        <p class="text-lg mb-6 opacity-90">Vismotion specializes in high-end video editing, motion graphics, and cinematic storytelling for brands, agencies, and creators.</p>
                        <p class="text-lg mb-8 opacity-90">With over 7 years of experience, we transform raw footage into compelling visual narratives that captivate audiences.</p>
                        <a href="#contact" class="inline-block border-2 border-accent text-accent px-8 py-3 rounded-full font-medium hover:bg-accent hover:text-primary transition-all">Get in touch</a>
                    </div>
                    <div class="md:w-1/2 animate-float">
                        <div class="relative">
                            <div class="absolute -inset-4 border-2 border-accent rounded-lg rotate-6"></div>
                            <img src="http://static.photos/black/640x360/1" alt="Vismotion Editor" class="relative rounded-lg shadow-2xl">
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Portfolio Section -->
        <section id="portfolio" class="py-20 bg-primary">
            <div class="container mx-auto px-6">
                <div class="text-center mb-16">
                    <h2 class="text-3xl md:text-4xl font-bold mb-4 animate-slide-up">Our <span class="text-accent">Work</span></h2>
                    <p class="text-lg opacity-90 max-w-2xl mx-auto animate-slide-up delay-100">Selected projects showcasing our editing expertise</p>
                </div>
                
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                    <!-- Project 1 -->
                    <div class="group relative overflow-hidden rounded-lg shadow-lg animate-slide-up delay-150">
                        <div class="aspect-w-16 aspect-h-9">
                            <video muted loop class="w-full h-full object-cover">
                                <source src="https://assets.mixkit.co/videos/preview/mixkit-waves-in-the-water-1164-large.mp4" type="video/mp4">
                            </video>
                        </div>
                        <div class="absolute inset-0 bg-gradient-to-t from-black/80 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end p-6">
                            <div>
                                <h3 class="text-xl font-bold mb-2">Oceanic Reflections</h3>
                                <p class="text-sm opacity-90 mb-4">Documentary film editing</p>
                                <a href="#" class="text-sm font-medium hover:text-accent transition-colors">View Project →</a>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Project 2 -->
                    <div class="group relative overflow-hidden rounded-lg shadow-lg animate-slide-up delay-200">
                        <div class="aspect-w-16 aspect-h-9">
                            <video muted loop class="w-full h-full object-cover">
                                <source src="https://assets.mixkit.co/videos/preview/mixkit-city-traffic-at-night-1083-large.mp4" type="video/mp4">
                            </video>
                        </div>
                        <div class="absolute inset-0 bg-gradient-to-t from-black/80 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end p-6">
                            <div>
                                <h3 class="text-xl font-bold mb-2">Urban Pulse</h3>
                                <p class="text-sm opacity-90 mb-4">Music video editing</p>
                                <a href="#" class="text-sm font-medium hover:text-accent transition-colors">View Project →</a>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Project 3 -->
                    <div class="group relative overflow-hidden rounded-lg shadow-lg animate-slide-up delay-250">
                        <div class="aspect-w-16 aspect-h-9">
                            <video muted loop class="w-full h-full object-cover">
                                <source src="https://assets.mixkit.co/videos/preview/mixkit-close-up-of-coffee-beans-1721-large.mp4" type="video/mp4">
                            </video>
                        </div>
                        <div class="absolute inset-0 bg-gradient-to-t from-black/80 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end p-6">
                            <div>
                                <h3 class="text-xl font-bold mb-2">Morning Ritual</h3>
                                <p class="text-sm opacity-90 mb-4">Commercial editing</p>
                                <a href="#" class="text-sm font-medium hover:text-accent transition-colors">View Project →</a>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="text-center mt-16 animate-slide-up delay-300">
                    <a href="#" class="inline-block border-2 border-accent text-accent px-8 py-3 rounded-full font-medium hover:bg-accent hover:text-primary transition-all">View All Projects</a>
                </div>
            </div>
        </section>

        <!-- Services Section -->
        <section class="py-20 bg-secondary">
            <div class="container mx-auto px-6">
                <div class="text-center mb-16">
                    <h2 class="text-3xl md:text-4xl font-bold mb-4 animate-slide-up">Our <span class="text-accent">Services</span></h2>
                    <p class="text-lg opacity-90 max-w-2xl mx-auto animate-slide-up delay-100">Comprehensive video editing solutions</p>
                </div>
                
                <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                    <!-- Service 1 -->
                    <div class="bg-primary p-8 rounded-lg shadow-lg hover:shadow-xl transition-shadow animate-slide-up delay-150">
                        <div class="w-16 h-16 bg-accent text-primary rounded-full flex items-center justify-center mb-6">
                            <i data-feather="film" class="w-8 h-8"></i>
                        </div>
                        <h3 class="text-xl font-bold mb-4">Video Editing</h3>
                        <p class="opacity-90 mb-4">Professional editing for commercials, music videos, documentaries, and social media content.</p>
                        <ul class="space-y-2 opacity-90">
                            <li class="flex items-center">
                                <i data-feather="check" class="w-4 h-4 mr-2 text-accent"></i>
                                <span>Color grading</span>
                            </li>
                            <li class="flex items-center">
                                <i data-feather="check" class="w-4 h-4 mr-2 text-accent"></i>
                                <span>Audio mixing</span>
                            </li>
                            <li class="flex items-center">
                                <i data-feather="check" class="w-4 h-4 mr-2 text-accent"></i>
                                <span>Motion graphics</span>
                            </li>
                        </ul>
                    </div>
                    
                    <!-- Service 2 -->
                    <div class="bg-primary p-8 rounded-lg shadow-lg hover:shadow-xl transition-shadow animate-slide-up delay-200">
                        <div class="w-16 h-16 bg-accent text-primary rounded-full flex items-center justify-center mb-6">
                            <i data-feather="sliders" class="w-8 h-8"></i>
                        </div>
                        <h3 class="text-xl font-bold mb-4">Post-Production</h3>
                        <p class="opacity-90 mb-4">Comprehensive post-production services to polish your footage to perfection.</p>
                        <ul class="space-y-2 opacity-90">
                            <li class="flex items-center">
                                <i data-feather="check" class="w-4 h-4 mr-2 text-accent"></i>
                                <span>Visual effects</span>
                            </li>
                            <li class="flex items-center">
                                <i data-feather="check" class="w-4 h-4 mr-2 text-accent"></i>
                                <span>Sound design</span>
                            </li>
                            <li class="flex items-center">
                                <i data-feather="check" class="w-4 h-4 mr-2 text-accent"></i>
                                <span>Title sequences</span>
                            </li>
                        </ul>
                    </div>
                    
                    <!-- Service 3 -->
                    <div class="bg-primary p-8 rounded-lg shadow-lg hover:shadow-xl transition-shadow animate-slide-up delay-250">
                        <div class="w-16 h-16 bg-accent text-primary rounded-full flex items-center justify-center mb-6">
                            <i data-feather="tv" class="w-8 h-8"></i>
                        </div>
                        <h3 class="text-xl font-bold mb-4">Motion Graphics</h3>
                        <p class="opacity-90 mb-4">Dynamic animations and graphics to elevate your visual storytelling.</p>
                        <ul class="space-y-2 opacity-90">
                            <li class="flex items-center">
                                <i data-feather="check" class="w-4 h-4 mr-2 text-accent"></i>
                                <span>Logo animations</span>
                            </li>
                            <li class="flex items-center">
                                <i data-feather="check" class="w-4 h-4 mr-2 text-accent"></i>
                                <span>Infographics</span>
                            </li>
                            <li class="flex items-center">
                                <i data-feather="check" class="w-4 h-4 mr-2 text-accent"></i>
                                <span>2D/3D animation</span>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

        <!-- Testimonials -->
        <section class="py-20 bg-primary">
            <div class="container mx-auto px-6">
                <div class="text-center mb-16">
                    <h2 class="text-3xl md:text-4xl font-bold mb-4 animate-slide-up">Client <span class="text-accent">Testimonials</span></h2>
                    <p class="text-lg opacity-90 max-w-2xl mx-auto animate-slide-up delay-100">What our clients say about our work</p>
                </div>
                
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                    <!-- Testimonial 1 -->
                    <div class="bg-secondary p-8 rounded-lg shadow-lg animate-slide-up delay-150">
                        <div class="flex items-center mb-6">
                            <img src="http://static.photos/people/200x200/1" alt="Client" class="w-12 h-12 rounded-full mr-4">
                            <div>
                                <h4 class="font-bold">Sarah Johnson</h4>
                                <p class="text-sm opacity-80">Creative Director, Luminary Films</p>
                            </div>
                        </div>
                        <p class="opacity-90 italic mb-6">"Vismotion transformed our documentary with their exceptional editing skills. Their attention to narrative flow and emotional pacing was remarkable."</p>
                        <div class="flex space-x-1 text-accent">
                            <i data-feather="star" class="w-4 h-4 fill-current"></i>
                            <i data-feather="star" class="w-4 h-4 fill-current"></i>
                            <i data-feather="star" class="w-4 h-4 fill-current"></i>
                            <i data-feather="star" class="w-4 h-4 fill-current"></i>
                            <i data-feather="star" class="w-4 h-4 fill-current"></i>
                        </div>
                    </div>
                    
                    <!-- Testimonial 2 -->
                    <div class="bg-secondary p-8 rounded-lg shadow-lg animate-slide-up delay-200">
                        <div class="flex items-center mb-6">
                            <img src="http://static.photos/people/200x200/2" alt="Client" class="w-12 h-12 rounded-full mr-4">
                            <div>
                                <h4 class="font-bold">Michael Chen</h4>
                                <p class="text-sm opacity-80">Marketing Director, Urban Beat</p>
                            </div>
                        </div>
                        <p class="opacity-90 italic mb-6">"The music video editing exceeded our expectations. Vismotion captured the energy and mood perfectly, delivering a final product that went viral."</p>
                        <div class="flex space-x-1 text-accent">
                            <i data-feather="star" class="w-4 h-4 fill-current"></i>
                            <i data-feather="star" class="w-4 h-4 fill-current"></i>
                            <i data-feather="star" class="w-4 h-4 fill-current"></i>
                            <i data-feather="star" class="w-4 h-4 fill-current"></i>
                            <i data-feather="star" class="w-4 h-4 fill-current"></i>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Contact Section -->
        <section id="contact" class="py-20 bg-secondary">
            <div class="container mx-auto px-6">
                <div class="flex flex-col md:flex-row gap-12">
                    <div class="md:w-1/2 animate-slide-up">
                        <h2 class="text-3xl md:text-4xl font-bold mb-6">Get In <span class="text-accent">Touch</span></h2>
<p class="text-lg mb-8 opacity-90">Ready to elevate your video content? Get in touch to discuss your project.</p>
                        <div class="space-y-6">
                            <div class="flex items-start">
                                <div class="w-10 h-10 bg-accent text-primary rounded-full flex items-center justify-center flex-shrink-0 mr-4">
                                    <i data-feather="mail" class="w-5 h-5"></i>
                                </div>
                                <div>
                                    <h4 class="font-bold mb-1">Email</h4>
                                    <a href="mailto:rajzxc1910@gmail.com" class="opacity-90 hover:text-accent transition-colors">rajzxc1910@gmail.com</a>
                                </div>
                            </div>
                            
                            <div class="flex items-start">
                                <div class="w-10 h-10 bg-accent text-primary rounded-full flex items-center justify-center flex-shrink-0 mr-4">
                                    <i data-feather="phone" class="w-5 h-5"></i>
                                </div>
                                <div>
                                    <h4 class="font-bold mb-1">Phone</h4>
                                    <a href="tel:+918780786861" class="opacity-90 hover:text-accent transition-colors">+91 8780786861</a>
                                </div>
                            </div>
                            
                            <div class="flex items-start">
                                <div class="w-10 h-10 bg-accent text-primary rounded-full flex items-center justify-center flex-shrink-0 mr-4">
                                    <i data-feather="instagram" class="w-5 h-5"></i>
                                </div>
                                <div>
                                    <h4 class="font-bold mb-1">Instagram</h4>
                                    <a href="https://instagram.com/yourinstagram" class="opacity-90 hover:text-accent transition-colors">@yourinstagram</a>
                                </div>
                            </div>
                        </div>
</div>
                    
                    <div class="md:w-1/2 animate-slide-up delay-100">
                        <form class="bg-primary p-8 rounded-lg shadow-lg">
                            <div class="mb-6">
                                <label for="name" class="block mb-2 font-medium">Your Name</label>
                                <input type="text" id="name" class="w-full px-4 py-3 bg-secondary border border-gray-700 rounded-lg focus:outline-none focus:ring-2 focus:ring-accent focus:border-transparent">
                            </div>
                            
                            <div class="mb-6">
                                <label for="email" class="block mb-2 font-medium">Email Address</label>
                                <input type="email" id="email" class="w-full px-4 py-3 bg-secondary border border-gray-700 rounded-lg focus:outline-none focus:ring-2 focus:ring-accent focus:border-transparent">
                            </div>
                            
                            <div class="mb-6">
                                <label for="project" class="block mb-2 font-medium">Project Type</label>
                                <select id="project" class="w-full px-4 py-3 bg-secondary border border-gray-700 rounded-lg focus:outline-none focus:ring-2 focus:ring-accent focus:border-transparent">
                                    <option value="">Select project type</option>
                                    <option value="commercial">Commercial</option>
                                    <option value="music-video">Music Video</option>
                                    <option value="documentary">Documentary</option>
                                    <option value="social-media">Social Media</option>
                                    <option value="other">Other</option>
                                </select>
                            </div>
                            
                            <div class="mb-6">
                                <label for="message" class="block mb-2 font-medium">Project Details</label>
                                <textarea id="message" rows="5" class="w-full px-4 py-3 bg-secondary border border-gray-700 rounded-lg focus:outline-none focus:ring-2 focus:ring-accent focus:border-transparent"></textarea>
                            </div>
                            
                            <button type="submit" class="w-full bg-accent text-primary py-3 px-6 rounded-lg font-medium hover:bg-opacity-90 transition-all">Send Message</button>
                        </form>
                    </div>
                </div>
            </div>
        </section>
    </main>
    
    <custom-footer></custom-footer>
    
    <script src="components/navbar.js"></script>
    <script src="components/footer.js"></script>
    <script src="script.js"></script>
    <script>
        feather.replace();
        
        // Intersection Observer for animations
        document.addEventListener('DOMContentLoaded', function() {
            const animateElements = document.querySelectorAll('.animate-slide-up, .animate-fade-in, .animate-float');
            
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('active');
                    }
                });
            }, {
                threshold: 0.1
            });
            
            animateElements.forEach(el => observer.observe(el));
        });
    </script>
<script src="https://huggingface.co/deepsite/deepsite-badge.js"></script>
</body>
</html>
