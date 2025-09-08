<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Modern UI Web Application</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #0f172a 0%, #1e293b 100%);
            color: #e2e8f0;
            line-height: 1.6;
            padding: 20px;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 30px;
            background: rgba(15, 23, 42, 0.8);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
        }
        
        header {
            text-align: center;
            margin-bottom: 40px;
            padding-bottom: 30px;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        h1 {
            font-size: 3.5rem;
            background: linear-gradient(90deg, #6366f1 0%, #ec4899 100%);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            margin-bottom: 15px;
            font-weight: 800;
        }
        
        .tagline {
            font-size: 1.5rem;
            color: #94a3b8;
            margin-bottom: 20px;
        }
        
        .badges {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin-top: 20px;
            flex-wrap: wrap;
        }
        
        .badge {
            padding: 8px 16px;
            border-radius: 50px;
            font-size: 0.9rem;
            font-weight: 600;
            display: flex;
            align-items: center;
            gap: 5px;
        }
        
        .badge-react {
            background: linear-gradient(90deg, #61dafb 0%, #087ea4 100%);
            color: #0f172a;
        }
        
        .badge-vite {
            background: linear-gradient(90deg, #a855f7 0%, #ec4899 100%);
            color: white;
        }
        
        .badge-tailwind {
            background: linear-gradient(90deg, #38bdf8 0%, #0ea5e9 100%);
            color: white;
        }
        
        h2 {
            font-size: 2.2rem;
            margin: 40px 0 20px;
            color: #f8fafc;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        h2 i {
            background: linear-gradient(90deg, #6366f1 0%, #ec4899 100%);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        
        p {
            margin-bottom: 20px;
            color: #cbd5e1;
            font-size: 1.1rem;
        }
        
        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }
        
        .tech-card {
            background: rgba(30, 41, 59, 0.5);
            border-radius: 16px;
            padding: 25px;
            display: flex;
            align-items: center;
            gap: 15px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .tech-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
        }
        
        .tech-icon {
            font-size: 2.5rem;
            flex-shrink: 0;
        }
        
        .tech-content h3 {
            font-size: 1.4rem;
            margin-bottom: 8px;
            color: #f1f5f9;
        }
        
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            margin: 30px 0;
        }
        
        .feature-card {
            background: rgba(30, 41, 59, 0.5);
            border-radius: 16px;
            padding: 25px;
            border-left: 4px solid;
            border-image: linear-gradient(90deg, #6366f1 0%, #ec4899 100%) 1;
        }
        
        .feature-card h3 {
            font-size: 1.3rem;
            margin-bottom: 15px;
            color: #f8fafc;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .preview {
            text-align: center;
            margin: 50px 0;
        }
        
        .preview-button {
            display: inline-block;
            padding: 15px 40px;
            background: linear-gradient(90deg, #6366f1 0%, #ec4899 100%);
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-weight: 600;
            font-size: 1.2rem;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            margin-top: 20px;
        }
        
        .preview-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(99, 102, 241, 0.3);
        }
        
        .footer {
            text-align: center;
            margin-top: 50px;
            padding-top: 30px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #94a3b8;
        }
        
        @media (max-width: 768px) {
            h1 {
                font-size: 2.5rem;
            }
            
            .tagline {
                font-size: 1.2rem;
            }
            
            .tech-grid, .features-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>🚀 Modern UI Web Application</h1>
            <p class="tagline">A sleek, responsive, and modern web application built with cutting-edge technologies</p>
            <div class="badges">
                <div class="badge badge-react"><i class="fab fa-react"></i> React.js</div>
                <div class="badge badge-vite"><i class="fas fa-bolt"></i> Vite</div>
                <div class="badge badge-tailwind"><i class="fas fa-paint-brush"></i> Tailwind CSS</div>
            </div>
        </header>
        
        <section>
            <h2><i class="fas fa-star"></i> Overview</h2>
            <p>This modern web application showcases a sleek, responsive design built with React.js, Vite, and Tailwind CSS. Its clean design, smooth animations, and engaging user experience make it a perfect reference or inspiration for future projects.</p>
        </section>
        
        <section>
            <h2><i class="fas fa-cogs"></i> Tech Stack</h2>
            <div class="tech-grid">
                <div class="tech-card">
                    <div class="tech-icon">
                        <i class="fas fa-bolt" style="color: #a855f7;"></i>
                    </div>
                    <div class="tech-content">
                        <h3>Vite</h3>
                        <p>Fast development build tool and bundler</p>
                    </div>
                </div>
                
                <div class="tech-card">
                    <div class="tech-icon">
                        <i class="fab fa-react" style="color: #61dafb;"></i>
                    </div>
                    <div class="tech-content">
                        <h3>React.js</h3>
                        <p>Component-based UI library for building user interfaces</p>
                    </div>
                </div>
                
                <div class="tech-card">
                    <div class="tech-icon">
                        <i class="fas fa-paint-brush" style="color: #38bdf8;"></i>
                    </div>
                    <div class="tech-content">
                        <h3>Tailwind CSS</h3>
                        <p>Utility-first CSS framework for rapid UI development</p>
                    </div>
                </div>
            </div>
        </section>
        
        <section>
            <h2><i class="fas fa-sparkles"></i> Features</h2>
            <div class="features-grid">
                <div class="feature-card">
                    <h3><i class="fas fa-palette"></i> Beautiful Sections</h3>
                    <p>Includes Hero, Services, Features, How It Works, Roadmap, Pricing, Header & Footer sections with modern design principles.</p>
                </div>
                
                <div class="feature-card">
                    <h3><i class="fas fa-mouse"></i> Parallax Animations</h3>
                    <p>Smooth effects triggered by mouse movement & scrolling for an immersive user experience.</p>
                </div>
                
                <div class="feature-card">
                    <h3><i class="fas fa-shapes"></i> Complex UI Geometry</h3>
                    <p>Custom circular feature displays, grid lines, and side lines with Tailwind CSS.</p>
                </div>
                
                <div class="feature-card">
                    <h3><i class="fas fa-th-large"></i> Latest UI Trends</h3>
                    <p>Modern layouts such as Bento Grids that follow current design trends.</p>
                </div>
                
                <div class="feature-card">
                    <h3><i class="fas fa-fill-drip"></i> Cool Gradients</h3>
                    <p>Stylish gradients applied to cards, buttons, and sections for visual appeal.</p>
                </div>
                
                <div class="feature-card">
                    <h3><i class="fas fa-mobile-alt"></i> Responsive Design</h3>
                    <p>Optimized for all screen sizes – desktop, tablet, and mobile devices.</p>
                </div>
                
                <div class="feature-card">
                    <h3><i class="fas fa-code"></i> Clean Code Architecture</h3>
                    <p>Reusable and well-structured code for easy maintenance and scalability.</p>
                </div>
            </div>
        </section>
        
        <section class="preview">
            <h2><i class="fas fa-eye"></i> Live Preview</h2>
            <p>Check out the live deployment of this modern web application</p>
            <a href="https://spiffy-spy.surge.sh" class="preview-button">
                <i class="fas fa-external-link-alt"></i> View Live Demo
            </a>
        </section>
        
        <div class="footer">
            <p>Made with ❤️ using modern web technologies</p>
        </div>
    </div>
</body>
</html>
